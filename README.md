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
stackexchange](http://tex.stackexchange.com/questions/146529/design-a-custom-beamer-theme-from-scratch).

I used it to learn how to make my own beamer themes.

Screenshots:

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

This package needs the [dvipsnames,usenames] options for beamer.

Screenshots:

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

### "LightRound"
My theme for the Lattice Conference 2015. It has some simple geometric shapes and matching boxes.

The colour theme I got from here (slightly modified)

https://color.adobe.com/Flat-UI-color-theme-2469224/?showPublished=true

Screenshots:

<table>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/light.round/screenshot-1.png" alt="Title Page" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/light.round/screenshot-2.png" alt="Items" width="400">
    </td>
  </tr>
  <tr>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/light.round/screenshot-3.png" alt="Boxes1" width="400">
    </td>
    <td>
      <img src="https://raw.githubusercontent.com/Irubataru/beamer-themes-screenshots/master/light.round/screenshot-4.png" alt="Boxes2" width="400">
    </td>
  </tr>
</table>

### "LightSquare"
Basically the same as LightRound, but with all the circles replaced with rectangles. Screenshots might follow.

### "CodeCourse"
The theme I used for the [C++ course](https://github.com/Irubataru/cpp-lecture-2015) I gave in 2015.

Font used for the examples: [Yanone Kaffeesatz Bold](http://www.yanone.de/typedesign/kaffeesatz/?key=typedesign/kaffeesatz)

Colours: [fresh cut day](http://www.colourlovers.com/palette/46688/fresh_cut_day) and [marty](http://www.colourlovers.com/color/FA2A00/marty)

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

## License

MIT

[screenshot-repo]: https://github.com/Irubataru/beamer-themes-screenshots
[talks-repo]: https://github.com/Irubataru/talks
