# MangaDex Limit Bypass

<div align="center">

[![GitHub Release](https://img.shields.io/github/v/release/m3chwj99/MangaDex-Limit-Bypass)](https://github.com/m3chwj99/MangaDex-Limit-Bypass/releases)
[![License](https://img.shields.io/badge/license-MIT-green)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-MangaDex-orange)](https://mangadex.org)
[![Tampermonkey](https://img.shields.io/badge/Tampermonkey-compatible-brightgreen)](https://www.tampermonkey.net/)
[![Violentmonkey](https://img.shields.io/badge/Violentmonkey-compatible-brightgreen)](https://violentmonkey.github.io/)
[![Greasy Fork](https://img.shields.io/greasyfork/v/579906)](https://greasyfork.org/fr/scripts/579906-mangadex-limit-bypass)
[![Installs](https://img.shields.io/greasyfork/dt/579906)](https://greasyfork.org/fr/scripts/579906-mangadex-limit-bypass)

</div>

A lightweight userscript that automatically resets the MangaDex guest page view limit, so you can keep reading without creating an account.

## How it works

MangaDex tracks the number of chapters you've read before displaying a pop-up that forces you to create an account or wait a certain amount of time before continuing, prompting you to create an account. This script periodically resets the number of chapters you've read so you don't hit a limit. 

## Installation
1. Install a userscript manager in your browser:
   - [Violentmonkey](https://violentmonkey.github.io/)
   - [Tampermonkey](https://www.tampermonkey.net/)

### Easy installation
1. Just install from [greasyfork](https://greasyfork.org/fr/scripts/579906-mangadex-limit-bypass)

### Manual installation
2. Create a new script and paste the contents of `mangadex-limit-bypass.user.js`

3. Save and make sure the script is enabled, that's it.

## Notes

- The script only runs on `https://mangadex.org/*`
- It does not interact with any external server
- It does not require any special permissions (`@grant none`)
- If `md-limit-data` is not found in localStorage, the script exits silently with a console error

## Disclaimer

This project is for educational purposes only. Use responsibly.