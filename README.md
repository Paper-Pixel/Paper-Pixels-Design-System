# Paper-Pixels-Design-System (Alpha)

Pixel Starter Package. This is compiling all of my custom styles I copy and paste around my projects. _Please feel free to copy, remix, submite a PR._ Right now this is optimized for my workflow and neuro thought patterns.

## Alpha Code

This code is in an Alpha state. Untill it settles down no promises on breaking changes. The first beta edition of this code will pay attention and work to not have breaking changes. Right now no such promises can be made.

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

The SASS files are written with the intent that any css class names declared in the HTML structure should be extending the styles declaired for semantic markup.

**HTML Markup**

```
    <section>
        <artical>
            <h1>I am a normal Title</h1>
            <h2 class='h1 bold'>
                I am a Title with the style of an h1 and bold text
            </h2>
        </artical>
    </section>
```

**PUG Markup**

```
    section
        artical
            h1 I am a normal Title
            h2(class='h1 bold') I am a Title with the style of an h1 and bold text
```

For maximum effect, I recomend altering the varibles located in the `source/styles/helpers/_variables.sass` file.

## Availible Varibles

#### Colors

`$color-white` Default White

`$color-primary` Primary Brand color

`$color-success` Secoundary & success Color
_This is a weird functionality, and should be updated to seperate these_

`$color-warning` Warning or Error color

`$color-light-base` Grey for use on top of the base color. _This needs to be refactored. The old version this came from was a nightmode site_

`$color-base` This is the darkest color in the pallet. _Needs to be refactored as the text color and background color need to be seperated_

`$color-grey` Default 3.0 contrast grey.

#### Typography

`$font-stack` This defines the default font stack for your site.

`$type-base-size` This defines the base measurements for the whole site. Changing this varible will have impact on padding, margins and type sizes.

`$type-ratios` An array of type ratios to choose from.

`$type-size-ratio` Sets the type ratio the dynamic font scale uses to scale fonts up from the `$type-base-size`.

`$type-levels` Defines how many header elements styles are going to be generated.

#### Transitions

`$transition-all` _Default_ transition all elements.

`$transition-hover` Transition of just the background element.

## Mixins

**The mixins for this project need to be refactored**

## Load Order

If you would like to update the order all of the parcel sass files load you can find them `source/styles/source.sass`

This will also let you add new Sass files to the load order.

# Working with the [PUG][pug-link] files

The PUG files are created as components. These components can be referenced and brought in to quickly build clean markup for your pages.

# Working with JS

No specail functions written for this yet. I would like to keep js down to a minimum for right now.

<!-- ======= Links ======= -->

[codekit-link]: https://codekitapp.com/
[pug-link]: https://pugjs.org/
[sass-link]: https://sass-lang.com/
