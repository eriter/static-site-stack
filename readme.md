# static-site-stack
[static-site-stack](https://github.com/wardpenney/static-site-stack)

A handy static site stack for getting off the ground instantly with SASS, HAML and Middleman. Assembled by [@wardpenney](http://twitter.com/wardpenney)

* [Middleman](http://middlemanapp.com/) Fantastic static sites
* [GroundworkCSS](http://groundwork.sidereel.com/) has an amazing SASS frontend grid
* [thin](http://code.macournoyer.com/thin/) web server

Also contains several optional things you can turn on:

* [Compass](http://compass-style.org/) SASS toolbox
* [Livereload](http://livereload.com/) Auto browser refresher
* [d3.js](http://d3js.org/) Data Representation Library
* [nvd3](http://nvd3.org/) A nice set of d3 graphs
* [jQuery](http://jquery.com/) Easy javascript

## Setup
Clone the static-site-stack into your own repository and GO!

```
git clone https://github.com/wardpenney/static-site-stack.git my_new_project_name
cd my_new_project_name
bundle
bundle exec middleman server
```
Then visit [localhost:4567](http://localhost:4567). Enjoy!


## Production Build
```
bundle exec middleman build
```
* Then deploy the build/ folder where you want! 

### Hosting Suggestions

* Registrar [DNSimple](https://dnsimple.com/) The best host ever for many reasons is actually pretty cheap also: **$3 for a couple of domains, or $8 for 10.**
* Host [Fjords](http://fjords.cc/) Is a static site host with deployment handy commands for Middleman. It's a steal of a deal: monthly **$4 plus $2 per domain**. And you can deploy with one command: `bundle exec middleman fjords --rebuild`

## Refernece
### Style Guide
There is a style guide at the /style route. I stongly suggest you add to it as you create new things. Style-guide only classes are prefixed with ".s-" and are contained in source/stylesheets/sections/_style.sass.
### Colors
I like to name my colors starting with $c- and then some name you choose. Often, I will use [ColourLovers.com](http://www.colourlovers.com) to create a palette, and this stack includes my [Alien Armor](http://www.colourlovers.com/palette/2871924/Alien_Armor) pallete by example. 

When you add / change colors, I suggest you follow the this convention:

1. Declare the color variable in source/stylesheets/libraries/_settings.sass
2. Add it to the two color classes utility lists in source/stylesheets/sections/_colors.sass

You will have the variable for use anywhere in the SASS codebase. Also you will get utility classes that begin with ".c-" for the CSS color rule and ".bc-" for the CSS background-color rule for use anywhere in the markup. 
### Font Faces
This site ships with Source Sans Pro as an example and uses my handy [bullet-proof font-face mixin](http://http://pivotallabs.com/bulletproof-font-face-syntax-with-sass/). Generally, I only include the weights as I need them and usually only end up with a few variants. To add fonts to your project:

1. Drop the files (.eot, .woff, .ttf, .svg) into the /source/fonts directory
2. Include a `declare-font-face(...)` line for each variant, making sure to assign the proper font-weight and font-style to each, but keeping them in the same font-family (see default implementation there as an example)
3. Declare a handy font-family variable in source/stylesheets/libraries/_settings.sass
4. Style at will!