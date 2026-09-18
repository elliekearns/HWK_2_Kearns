# CPSC 1710 Labs

Student-facing assignments and starter materials for CPSC 1710, Fall 2026.

## Labs

- [Lab 1: Meet a deep-learning notebook](lab-01/)
- [Lab 2: From one pixel to your classifier](lab-02/)

Use the [live course hub](https://xiuyechen.github.io/cpsc1710-labs/) for the simplest experience. Each assignment is available as a webpage and a printable PDF.

## Opening the files

The HTML files have no build step. After cloning, open `index.html` directly in Chrome, Safari, or Firefox. Avoid VS Code's **Open Preview** for these files: its internal `file+.vscode-resource` links do not work as normal browser addresses.

You can also serve the repository locally:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000/`.

## Classifier Development Log

I asked for a first version with three inputs.
The predictions were not very interesting or informative, so I added more labels.
I asked Codex to make the "What is this Teaching?" section more robust, instead of simply describing the concept of pattern matching.
I then asked Codex to make a few stylistic edits to improve readability.
Finally, I asked a friend to try it and __.


## Credits

Materials are by [Xiuye Chen](https://github.com/xiuyechen), developed with Codex, and shared under [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
