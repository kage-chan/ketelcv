<p align="middle">
<img src="https://github.com/kage-chan/ketelcv/blob/main/ScreenshotP1.png" width="300px"><img src="https://github.com/kage-chan/ketelcv/blob/main/ScreenshotP1.png" width="300px">
</p>

# ketelcv
Modern, flexible and easy-to-use LaTeX template for a cv

This year's version is ketelcv2024.sty, the accompanying examples for the file are main2024.tex and mainDE_2024.tex for the german version.

# Why?

I've been trying to keep my CV updated in the last years. A few years ago I found a LaTeX template I've changing here and there. The number of warnings was substantial, each time I wanted to change something it basically fell apart. So, this year I decided to give my template an overhaul, optically as well as technically. I've built a completely modular template for a CV that includes functions and blocks for all things I need for my CV.

# Usage
As compiler please use XeLaTeX. Other compilers might work, but I haven't tested any other compiler and I don't support them.

## Basics
For basic usage, simply use the example files (main2024.tex and mainDE_2024.tex) and fill in your details.
All functions, styles and settings are inside the first roundabout 100 lines in ketelcv2024.sty.

## Colors
To change the colors of the template for your needs, change the definitions in the block "COLORS" in the sty file.
The colors per default are defined as comma separated Red, Green and Blue (RGB) values. Other modes are available, check out the "xcolor" package documentation.

## Fonts
Unless you define a font, the default is Montserrat. If you want to change the font, you need to define three variables:
- \cvMainFont
- \cvMainItalicFont
- \cvMainBoldFont
You can find these three variables in the "FONT OPTIONS" section in the sty file. I have put examples for using TTF or OTF files in there, too.

> [!CAUTION]
> If you change the font, things WILL move around and could (unlikely, but could) break. Please only change the font if you're willing to play with the margins and vspaces within the functions.


# Kown issues and problems
1. Not an issue as such, but something that might happen: Should you get an error that mumbles something about an "missing \item" or something and you're getting big blank portions on a page, your text is most likely running into the bottom margin before you issue the \newpage command. You need to either adjust your text sizes or text length to avoid running into the bottom margin.
