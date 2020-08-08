# Paper-Pixels-Design-System (Alpha)

Pixel Starter Package. This is compiling all of my custom styles I copy and paste around my projects. _Please feel free to copy, remix, submite a PR_ Right now this is optimized for my workflow and neuro thought patterns.

## How is this built?

HTML is being compiled from [PUG][pug-link] and CSS is being compiled from [SASS][sass-link], Still just using Vanilla Javascript with a sprinkeling of ES6.

All of these langueges are being compiled with [CodeKit][codekit-link].

# Getting Started

I do not have this set up as a template or packege yet. To hit the ground running;

1. Clone the repo to your computer
2. Define what your needs are
   2a. Use _compiled code in the build folder_ if you only need a CSS framework to work with.
   2b. Use [PUG][pug-link] & [SASS][sass-link] files to quickly build up your own site.

# Working with the [SASS][sass-link] files

For maximum effect, I recomend altering the varibles located in the `source/styles/helpers/_variables.sass` file.

## Availible Varibles

_Colors_
`$color-white` Default White

`$color-primary` Primary Brand color

`$color-success` Secoundary & success Color
_This is a weird functionality, and should be updated to seperate these_

`$color-warning` Warning or Error color

`$color-light-base` Grey for use on top of the base color. _This needs to be refactored. The old version this came from was a nightmode site_

`$color-base` This is the darkest color in the pallet. _Needs to be refactored as the text color and background color need to be seperated_

`$color-grey` Default 3.0 contrast grey.

<!-- ======= Links ======= -->

[codekit-link]: https://codekitapp.com/
[pug-link]: https://pugjs.org/
[sass-link]: https://sass-lang.com/
