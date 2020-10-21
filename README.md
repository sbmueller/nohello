# Nohello

This is the source of [this](https://sbmueller.github.io/nohello/) website.

## Build

There is a Github Action in place to deploy any changes to `index.md` to the
`index.html` site when pushing to `master` branch.

To generate the HTML file from Markdown manually,
[pandoc](https://github.com/jgm/pandoc) is used:

```
pandoc --standalone --metadata pagetitle="nohello" --css "assets/css/pandoc.css" --output=index.html index.md
```

## Acknowledgements

This website was inspired by the original at
[nohello.com](https://www.nohello.com/). Acknowledgements go to the original
anonymous author. I felt an urge to modernize this gem with a more suitable
layout, https connection and open-sourced code.
[Stylesheet](https://gist.github.com/forivall/7d5a304a8c3c809f0ba96884a7cf9d7e#file-gh-pandoc-css)
licensed under MIT license, Copyright (c) 2016-2017 Emily M Klassen.
