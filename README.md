Sass Slate Toolkit
=============

A **SCSS** boilerplate for creating themes in [SlateCMS](http://slatecms.wvu.edu).

## What's included?
 * `.rhtml` files for native development within the CMS.
 * A `scss` folder for everything you need to hit the ground running with Sass.
 * `.html` files for those who prefer to work in flat HTML and convert to `.rhtml` (or whatever else) later. 
 * A Photoshop file with some basic typography, grid layout, WVU's global masthead and footer. 
 * A swatches file for Photoshop that contains the WVU brand colors.


## How do I use it?
1. [Download the zip](https://github.com/wvuweb/slate-toolkit/archive/scss.zip).  
2. Use the `.rhtml` files (or convert those to normal HTML).
3. Drag your project's folder onto [CodeKit](http://incident57.com/codekit/index.php) ([Prepros](http://alphapixels.com/prepros/), [Mixture](http://mixture.io), [Scout](http://mhs.github.io/scout-app/), or any other precompiler will also work).
4. We bundle Compass by default. To get that working in CodeKit: 
    * Right click your project on the left side of CodeKit and select "Compass > Use Compass for this project".
    * Select "Locate" in the modal that appears.
    * Select the `config.rb` file in your project's root folder and hit "OK". 
5. Develop your site, upload to Slate (or wherever) like you always have, and prosper.

For instructions on how to use the Fluid Mobile First Skeleton Grid, please refer to [its repository](https://github.com/adamjohnson/Skeleton-fluid-mobile-first) or the [Skeleton homepage](http://www.getskeleton.com/).

### Features
 * Pick and choose what Sass partials you want. Use all, some, or none. We've made it modular—letting you choose which files you want and which you don't.
     * Check out `styles.scss` and `slate_themes/shared/scss/` to pick and choose which files you want to include. 
 * HTML5 Ready
 * Fluid and mobile first using the [Fluid Mobile First Skeleton Grid](https://github.com/adamjohnson/Skeleton-fluid-mobile-first)
 * Compatible with [all of the browsers that we support](https://brand.wvu.edu/web_standards).
 * Includes [WVU's global stylesheet](http://slate.wvu.edu/themes/shared/scss/v4/stylesheets/global-v4.css) which has [Normalize.css](http://necolas.github.io/normalize.css/), basic print styles, WVU's global masthead, footer, and typography baked right in.
 * Built with progressive enhancement in mind.
 * Placeholder CSS Media Queries
 * and so much more...

### "I want to customize this boilerplate. What's the best way to do that?"
Enter into the world of forking with Git. At the top of this page is a "Fork" button. This will copy (or "`fork`") this repository to your account. From there, you can use Git & GitHub to customize this toolkit to your liking. If we make a change later that you like and want to add to your customized version, [it's super easy](https://help.github.com/articles/fork-a-repo). If you need help learning Git, check out [Try Git](http://try.github.io). 

#### What's with the `partials`, `utilities`, and `vendor` folders?
This is meant to be a way to keep your project organized and well structured. It's based off of concepts from [this post](http://thesassway.com/beginner/how-to-structure-a-sass-project).

  * The `partials` directory is where the majority of your CSS will be constructed. A lot of folks enjoy breaking their stylesheets into sections like header, sidebar, footer, etc. The way your organize your project is up to you.
  * The `utilities` folder is for mixins and other Sass code that doesn't actually output CSS. 
  * The `vendor` directory is for third party CSS. Any CSS coming from third party sources (such as FlexSlider, Bootstrap, etc) should go in this folder. CSS in the vendor folder should not be edited. If you edit it, immediately move it to the `partials` folder.

#### Whaaaaaat?!? No `scss` folder for flat HTML Projects? What gives, dude?
Not to worry! We didn't want to have to maintain the `scss` folder in two places; thereby, why we kept the `scss` files in the `html5_rhtml` folder. If you want to use the scss folder in a flat HTML project, simply copy and paste the `scss` folder from the `html5_rhtml` directory to the `html5_html` directory.