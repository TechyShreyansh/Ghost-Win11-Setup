# 🚀 Fastfetch Custom Setup

A **professional, clean, and aesthetic Fastfetch configuration** for
Linux users.\
Designed for developers who want a minimal yet powerful system fetch
display with **custom icons and image/logo support**.

------------------------------------------------------------------------

## ✨ Preview

Minimal • Fast • Professional • Custom Image Support

------------------------------------------------------------------------

## 🧩 Features

-   🎨 Nerd Font based **custom icons**
-   🖼️ **Image / Logo rendering** (Kitty & Konsole supported)
-   ⚡ Optimized Fastfetch layout
-   🧼 Clean & minimal design
-   🛠️ Easy to customize and extend

------------------------------------------------------------------------

## 🛠️ Installation

### 🔹 Prerequisites

Make sure these packages are installed:

#### Arch / Arch-based Linux

``` bash
sudo pacman -S fastfetch imagemagick ttf-jetbrains-mono-nerd
```

> ⚠️ ImageMagick is required for image rendering.

------------------------------------------------------------------------

### 🔹 Quick Setup

``` bash
# Clone the repository
git clone https://github.com/TechyShreyansh/Fastfetch-Config.git
cd Fastfetch-Config

# Backup existing configuration (optional)
mv ~/.config/fastfetch ~/.config/fastfetch_backup

# Copy new configuration
cp -r fastfetch ~/.config/
```

------------------------------------------------------------------------

### 🔹 Terminal Configuration

For icons to appear correctly, set your terminal font to:

    JetBrainsMono Nerd Font Mono
    
    sudo pacmn -S ttf-jetbrains-mono-nerd
    
    fc-cache -fv

✅ This step is mandatory, otherwise icons may not appear.

Recommended Terminals: - Kitty ✅ - Konsole ✅

------------------------------------------------------------------------

## 🖼️ Custom Image / Logo Setup

You can replace the default logo with your own image.

### Step 1: Add Image

Copy your image (PNG/JPG) into:

    ~/.config/fastfetch/

### Step 2: Edit Config

Open the config file:

    ~/.config/fastfetch/config.jsonc

### Step 3: Update Logo Section

``` json
"logo": {
  "type": "kitty",
  "source": "/home/username/.config/fastfetch/logo.png",
  "width": 25,
  "height": 12
}
```

### 📝 Notes

-   Kitty users → `"type": "kitty"`
-   Konsole users → `"type": "iterm"` or `"sixel"`
-   Always use **full image path**
-   Adjust width & height for best appearance

------------------------------------------------------------------------

## 🧪 Usage

Run Fastfetch:

``` bash
fastfetch
```

------------------------------------------------------------------------

## ❤️ Credits

Maintained by **Tech Shreyansh**\
Telegram & YouTube: **youtube.com/@TechShreyansh**

------------------------------------------------------------------------

## ⭐ Support

If you like this setup, don't forget to **star the repository** ⭐
