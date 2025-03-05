# MeDA Lab Slide Template

This repository contains a [Typst](https://typst.app/) template for creating slides for MeDA Lab.

## Getting Started

### Installation

1. Install the [Typst](https://typst.app/) and Tinymist VSCode extensions.
2. Clone this repository:
    ```bash
    git clone https://github.com/yenjia/meda-typst.git
    ```
3. Import the template:
    - To use the template in the same working directory, refer to `main.typ`.
    - To use the template as a package, move the folder to `$HOME/.local/share/typst/packages/local/`:
    ```bash
    cp -r meda-typst/* $HOME/.local/share/typst/packages/local/meda-typst/0.1.0/
    ```
### How to Use
There are 6 kinds of slides in the template (See `main.typ` for more details):
1. Front slide
```typst
#front-slide(
  title: "Slide",
  subtitle: "Online Meeting || 2025/00 00:00",
  authors: "Your name",
  info: [MeDA Lab || Degree Program of Data Science],
  theme: "", // none, bluey, greeny, reddy, dusky
)
```
2. Title slide
```typst
#title-slide[This in the title]
```
3. Normal slide
```typst
#slide(title: "Title")[
    - xxx
    - yyy
    - zzz
]
```
4. Blank slide
```typst
#blank-slide[
    - xxx
    - yyy
    - zzz
]
```
5. Bibliography slide
```typst
#let bib = bibliography("bibliography.bib")
#bibliography-slide(bib)
```
6. End slide
```typst
#end-slide[Q & A]
```

## Notes

I adjusted the template based on my own preferences, so the settings for position, font size, etc., are different from the version in the slide. You can adjust them as needed 🤡.
