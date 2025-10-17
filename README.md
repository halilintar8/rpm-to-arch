# rpm-to-arch

A small utility to convert **.rpm (Red Hat / Fedora)** packages into **Arch Linux packages** (`.pkg.tar.zst`).

This project is based on and modified from the original code by [zinovyev](https://gist.github.com/zinovyev/0ad6bd54ac5a9f7b709607a8151a0334).

---

## 📦 Overview

`rpm-to-arch` automates the process of repackaging `.rpm` files for use on Arch Linux–based systems.  
It simplifies converting RPM packages into installable Arch packages using `makepkg` and `PKGBUILD`.

---

## 🔧 Requirements

Before using, ensure you have:

- `bash`
- `rpmextract` or `bsdtar`
- `makepkg` (from `base-devel` group)
- `gzip`, `xz`, or `zstd` depending on your packaging format

Install required tools on Arch Linux:

```bash
sudo pacman -S base-devel rpmextract

