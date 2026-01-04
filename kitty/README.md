# Kitty Terminal Configuration

This repository contains my personal configuration for the **Kitty terminal emulator**.
The setup is optimized for clarity, readability, and long coding sessions.

---

## Font: Iosevka

**Iosevka** is an open-source typeface family designed specifically for technical use.

> Iosevka [ˌjɔˈseβ.kʰa] is an open-source, sans-serif + slab-serif, monospace + quasi-proportional typeface family, designed for writing code, using in terminals, and preparing technical documents.

It provides:
- Excellent readability in terminals
- High customizability
- Clear distinction between similar characters
- Suitable balance for long-term coding and technical work

This configuration uses **Iosevka** as the primary terminal font.

---

## Installing Iosevka Font

### Download from GitHub Releases

You can download the font packages directly from the official GitHub releases.

For **Linux users**, the following command downloads all TTC packages from the latest release:

```bash
curl -s 'https://api.github.com/repos/be5invis/Iosevka/releases/latest' | jq -r ".assets[] | .browser_download_url" | grep PkgTTC-Iosevka | xargs -n 1 curl -L -O --fail --silent --show-error
```

### Installation Steps

After downloading:

1. **Quit all editors and terminal programs**
2. **Extract** the downloaded font archive
3. Install the fonts based on your operating system:

#### Windows

* Select the font files and drag them into **Font Settings** or the **Font Control Panel**
* On **Windows 10 (1809+)**, fonts are installed per-user by default
  For better compatibility (especially with Java-based apps):

  * Right-click the font files
  * Select **Install for all users**

#### macOS

* Follow the standard macOS font installation process
  (Double-click the font files and install via Font Book)

#### Linux

* Copy the font files into your fonts directory:

  ```bash
  ~/.fonts
  ```

  or

  ```bash
  ~/.local/share/fonts
  ```
* Then rebuild the font cache:

  ```bash
  fc-cache -fv
  ```

---

## Usage

Once the font is installed:

* Kitty will automatically use it according to the configuration in this repository
* Restart Kitty to apply changes

---

## Notes

* This repository focuses **only** on terminal configuration
* No GUI theming or unrelated system tweaks are included
* The goal is a clean, distraction-free terminal environment