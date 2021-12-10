## Was this written from scratch?
This library combines the following:
- reset.css 2.0 by Eric Meyer
- normalize.css 8.0.0 by Nicolas Gallagher and Jonathan Neal 
- The Bootstrap 4 Reboot CSS

This library adds standardizations onto the above

## What is css-baseline?
Browers come with different default CSS styles, this library tries to provide a common style starting point so that html appears and behaves the same in all browsers. It is especially geared towards fixing edge-case bugs/behaviors (*cough* *cough* IE 9,10,11 *cough* *cough*). There are no CSS-classes since it this is intended to be used with other style sheets / CSS frameworks.<br>
<br>
The goal is that CSS baseline can be used as a foundation for all future web-dev projects regardless of anyone's project-specific styling needs.

## How do I use this?
Make sure you include this CSS __before__ any other style sheets: this lets other libraries override css-baseline
1. __[quick way]__ If you're just testing you can paste this in the \<head> of your HTML file.<br>
`<link rel="stylesheet" href="https://unpkg.com/css-baseline/css/2.css">`
2. __[better way]__ You can also manually download the CSS file of version you want (see the `css` folder). Then just include it as the first style sheet in the \<head> of your HTML file.
3. __[best way]__ If you have a bundler in your project (e.g. Parcel.js, Webpack, Rollup.js) you can include this through npm.<br>
Ex: In your main/first javascript file you can likely put `require("css-baseline/css/2")` or `import "css-baseline/css/2"`. Your bundler may have some other way of including CSS files from NPM.

## Why are their 4 versions?
Versions:
1. Only include critical fixes
2. Standardize the spacing of elements (and everything from #1)
3. Standardize font sizing and scroll bars (and everything from #1 and #2)
4. Standardize the look of buttons and text-input fields (and everything from #1, #2, and #3)

## Is this going to be updated?
Yes. Please create pull requests if any browsers have non-standard behavior/bugs that can be fixed with CSS or if there is any conflict with major libraries.
