# What is css-baseline?
This is a library that is designed to be an unopinionated standardization/normalization of CSS defaults across browsers, especially including fixing edge-case bugs/behaviors (*cough* *cough* IE 9,10,11 *cough* *cough*). There are no CSS-classes in this library since it is strictly for setting defaults. The code in general is indended to be used with other style sheets / CSS frameworks.<br>
<br>
The goal is that CSS baseline can be used as a foundation for all future web-dev projects regardless of anyone's project-specific styling needs.

## How do I use this?
1. [quick] If you're just testing you can paste this in the <head> of your HTML file.<br>
`<link rel="stylesheet" href="https://unpkg.com/css-baseline/css/4.css">`
2. [better] You can also manually download the css file of version you want (see the `css` folder). Then just include it as the first style sheet in the <head> of your HTML file.
3. [best] If you have a bundler in your project (e.g. Parcel.js, Webpack, Rollup.js) you can include this through npm.<br>
Ex: In your main/first javascript file you can likely put `require("css-baseline/css/5")` or your bundler may have some other way of including css files from NPM.


## Why are their 5 versions?
The versions are a gage of how 'standardized' you'd prefer to start off.<br>
Number 4 is the reccomended version.
1. Only include critical fixes
2. Standardize the spacing of elements (and everything from #1)
3. Standardize font sizing (and everything from #1 and #2)
4. Standardize buttons and text-input fields (and everything from #1, #2, and #3)
5. Make things fancy (animation) (and everything from #1, #2, #3, and #4)

## Is this going to be updated?
Yes, please post pull requests if any browsers have non-standard behavior/bugs that can be fixed with CSS.

## Are there future plans for more features?
Yes, #5 and #4 will likely have additional functionality added to them. It will be visibly minimal, and will probably involve more obscure elements like details, legends, fieldsets, etc. There is also a plan for a very large addition of baseline-#6 which will include standardizations that require javascript.
