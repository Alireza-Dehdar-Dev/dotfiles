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
curl -s 'https://api.github.com/repos/be5invis/Iosevka/releases/latest' \
| jq -r ".assets[] | .browser_download_url" \
| grep PkgTTC-Iosevka \
| xargs -n 1 curl -L -O --fail --silent --show-error

