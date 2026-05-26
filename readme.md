# MangaDex Limit Bypass

A lightweight userscript that automatically resets the MangaDex guest page view limit, so you can keep reading without creating an account.

## How it works

MangaDex tracks the number of chapters you've read before displaying a pop-up that forces you to create an account or wait a certain amount of time before continuing, prompting you to create an account. This script periodically resets the number of chapters you've read so you don't hit a limit. 

## Installation

1. Install a userscript manager in your browser:
   - [Violentmonkey](https://violentmonkey.github.io/)
   - [Tampermonkey](https://www.tampermonkey.net/)

2. Create a new script and paste the contents of `mangadex-limit-bypass.user.js`

3. Save and make sure the script is enabled, that's it.

## Configuration (if you want)

At the top of the script, you can adjust the threshold before the reset kicks in:

```js
const maxChapterLimit = 5; // reset when counter exceeds this value
```

## Notes

- The script only runs on `https://mangadex.org/*`
- It does not interact with any external server
- It does not require any special permissions (`@grant none`)
- If `md-limit-data` is not found in localStorage, the script exits silently with a console error

## Disclaimer

This project is for educational purposes only. Use responsibly.