# Gentoo Linux Configuration (Intel i9 285K & RTX 5090 & Sway)

My personal Gentoo Linux configuration files, optimized for the Intel Core Ultra 9 285K hybrid architecture, an ASUS ROG Astral NVIDIA GeForce RTX 5090, and a minimalist Wayland desktop environment using Sway.

## 💻 System Specifications
*   **CPU:** Intel Core Ultra 9 285K (Arrow Lake - 24 cores / 24 threads)
*   **GPU:** ASUS ROG Astral NVIDIA GeForce RTX 5090 (32GB GDDR7)
*   **Motherboard:** ASUS ROG Maximus Z890 Hero
*   **Display Server:** Wayland
*   **Window Manager:** Sway (i3-compatible Wayland compositor)
*   **Init System:** OpenRC

## 🛠️ Highlights & Features
*   **Arrow Lake Optimizations:** Fine-tuned `march=arrowlake` and `COMMON_FLAGS` in `make.conf` to effectively leverage the hybrid Performance/Efficient core design.
*   **Blackwell GPU Setup:** Pre-configured `VIDEO_CARDS="nvidia"` with the mandatory `USE="kernel-open"` flag required for modern RTX 50-series hardware support.
*   **Sway & Wayland Ready:** Pure Wayland environment; X11 dependencies and bloat stripped globally.
*   **LUKS Encryption:** Pre-configured secure disk encryption layout handled cleanly via OpenRC `dmcrypt`.
*   **Clean Portage Structure:** Split configuration using structured directories for `package.use/`, `package.accept_keywords/`, and `package.mask/`.

## 🚀 How to Use
> ⚠️ **Warning:** Do not blindly copy these files. Review them thoroughly and adjust the configurations to match your precise storage layout and peripheral components.

Clone this repository:
```bash
git clone https://github.com/tabaluga-crypto/gentoo-config/tree/main
```

## 📝 License
This repository is open-source and available under the [MIT License](LICENSE).
