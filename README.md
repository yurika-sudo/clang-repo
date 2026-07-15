# Android Clang Toolchains Mirror

A manual/automated mirror repository for compiled Clang/LLVM toolchains used in Android kernel (GKI/CLO) compilation. 

This repository fetches prebuilt toolchains from their original sources and re-hosts them via GitHub Releases. The primary goal is to provide faster, more stable download links and prevent timeout issues when syncing toolchains across various CI/CD environments (like GitHub Actions).

## 📦 Included Toolchains

### Google Official Prebuilts (AOSP)
* **Clang r450784e** (LLVM 14)
* **Clang r522817** (LLVM 18)
* **Clang r547379** (LLVM 20)
* **Clang r563880c** (LLVM 21)
* **Clang r584948b** (LLVM 22)

### ZyCromerZ Custom Toolchains
* **ZyC Clang 14.0.6** (LLVM 14)
* **ZyC Clang 23.0.0git** (LLVM 23)

## 🤝 Credits & Acknowledgments

This repository **does not** compile these toolchains from source. All binaries are mirrored directly from their respective creators. Massive thanks and full credits go to:

* **[Google / Android Open Source Project](https://android.googlesource.com/platform/prebuilts/clang/host/linux-x86/)** for the official AOSP Clang toolchains.
* **[ZyCromerZ](https://github.com/ZyCromerZ/Clang)** for the highly optimized custom LLVM/Clang builds.

## ⚙️ Usage
You can fetch the toolchains directly from the [Releases](../../releases) tab using `wget`, `curl`, or `aria2c` in your kernel build scripts.

```bash
# Example: Downloading ZyC Clang 14.0.6
wget [https://github.com/YOUR_USERNAME/YOUR_REPO_NAME/releases/download/YOUR_TAG/ZyC-Clang-14.0.6.tar.gz](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME/releases/download/YOUR_TAG/ZyC-Clang-14.0.6.tar.gz)
