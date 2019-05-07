# beamer-themes

This is a collection of beamer themes I have made.

They are not "industry grade", so expect various quirks. I am still learning to
develop these, and I will hopefully get better with time. Most of all I hope
that the code might give someone else some pointers to get them started
developing their own themes.

## Themes

These are the themes available at the moment. The screenshots are stored in a
[separate repo][screenshot-repo] which you can also check out for the TeX-files
used to generate them. If you want to see examples of use then [check out the
various talks I have given][talks-repo] as I in most scenarios made use of these
themes when making them.

### "corporate"

This is a simple blue and orange theme inspired by [the following post on
stackexchange][stackexchange-post].

I used it to learn how to make my own beamer themes.

#### Screenshots

<table>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/corporate/screenshot-1.png" alt="Title Page" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/corporate/screenshot-2.png" alt="Items" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/corporate/screenshot-3.png" alt="Boxes" width="400">
    </td>
  </tr>
</table>

### "cleancode"
The theme I prefer to use when giving a programming-related talk. It is mostly empty and has 
overloaded boxes that I find pleasing.

This package needs the `[dvipsnames,usenames]` options for beamer.

```tex
\documentclass[dvipsnames,usenames]{beamer}
```

#### Screenshots

<table>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/clean.code/screenshot-1.png" alt="Title Page" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/clean.code/screenshot-2.png" alt="Items" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/clean.code/screenshot-3.png" alt="Boxes1" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/clean.code/screenshot-4.png" alt="Boxes2" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/clean.code/screenshot-5.png" alt="Boxes3" width="400">
    </td>
  </tr>
</table>

### "LightTheme"
My theme for the Lattice Conference 2015. It has some simple geometric shapes and matching boxes.

It was originally known as "LightRound" (or "LightSquare"), but these have been
removed in favour of this theme which can produce both of them. On top of the
regular [configurations](#configuration) there is also a flag which changes the shapes in the
various banners. The flag is called `shape` and can be
 - `circle` (default)
 - `square`
 - `pentagon`
 - `hexagon`
 - `septagon`
 - `octagon`

```tex
\usetheme[shape=circle]{LightTheme} % Identical to using LightRound
\usetheme[shape=square]{LightTheme} % Identical to using LightSquare
```

The colour theme is a slight modification on a theme called [Flat UI][flat-ui-theme].

#### Screenshots

<table>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/light.theme/screenshot-1.png" alt="Title Page" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/light.theme/screenshot-2.png" alt="Section page" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/light.theme/screenshot-3.png" alt="Items" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/light.theme/screenshot-4.png" alt="Boxes1" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/light.theme/screenshot-5.png" alt="Boxes2" width="400">
    </td>
  </tr>
</table>

### "CodeCourse"

The theme I used for the [C++ course](https://github.com/Irubataru/cpp-lecture-2015) I gave in 2015.

The theme is configured to use the following two fonts:
  - [Yanone Kaffeesatz][yanone-kaffeesatz]
  - [Fira Code][fira-code]

The colours are:
 - Theme [fresh cut day](https://www.colourlovers.com/palette/46688/fresh_cut_day)
 - Colour [marty](http://www.colourlovers.com/color/FA2A00/marty)

#### Screenshots

<table>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/code.course/screenshot-1.png" alt="Title Page" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/code.course/screenshot-2.png" alt="Items" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/code.course/screenshot-3.png" alt="Boxes1" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/code.course/screenshot-4.png" alt="Boxes2" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/code.course/screenshot-5.png" alt="Boxes1" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/code.course/screenshot-6.png" alt="Boxes2" width="400">
    </td>
  </tr>
</table>

## Configuration

I have tried my best to use the standard beamer names for the colours and fonts,
but if anything is off then you can read the sources in [color](color) to see
which name I have used.

All of the themes have a flag you can use to change the slide numbering format.
The key is named `numbering` and has three options:

 - `none` no numbering
 - `counter` a simple page count
 - `fraction` current page / total pages

```tex
\usetheme[numbering=none]{LightTheme}
\usetheme[noslidenumbes]{LightTheme} % Same as numbering=none
```

## Installation

Standard LaTeX installation, put the files somewhere LaTeX can find them. I normally put these in

```bash
$TEXMFHOME/tex/latex/beamer/themes/
```

You can also achieve the same effect by adding the repo path to your `TEXINPUTS`
environment variable, e.g. through:

```bash
export TEXINPUTS=/path/to/repo//:$TEXINPUTS
```

Note the extra `//` at the end of the path as it tells latex to include files
recursively.

## Inspiration

 - [This stackexchange post is what got me started][stackexchange-post]
 - [mtheme][mtheme] has been an invaluable source of examples for how certain
   things can be carries out in latex and beamer

## License

MIT

[screenshot-repo]: https://github.com/Irubataru/beamer-themes-screenshots
[talks-repo]: https://github.com/Irubataru/talks
[stackexchange-post]: http://tex.stackexchange.com/questions/146529/design-a-custom-beamer-theme-from-scratch
[flat-ui-theme]: https://color.adobe.com/Flat-UI-color-theme-2469224/?showPublished=true
[yanone-kaffeesatz]: http://www.yanone.de/typedesign/kaffeesatz/?key=typedesign/kaffeesatz
[fira-code]: https://github.com/tonsky/FiraCode
[mtheme]: https://github.com/matze/mtheme
