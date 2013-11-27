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
```
git clone https://github.com/wardpenney/static-site-stack.git
bundle install
bundle exec middleman server
```
Then visit [localhost:4567](http://localhost:4567). Enjoy! And don't forget to turn on your LiveReload [Chrome Browser Extension](https://chrome.google.com/webstore/detail/livereload/jnihajbhpnppcggbcgedagnkighmdlei?hl=en)!


## Production Build
```
bundle exec middleman build
```
* Then deploy the build/ folder where you want! 

### Hosting Suggestions

* Registrar [DNSimple](https://dnsimple.com/) The best host ever for many reasons is actually pretty cheap also: **$3 for a couple of domains, or $8 for 10.**
* Host [Fjords](http://fjords.cc/) Is a static site host with deployment handy commands for Middleman. It's a steal of a deal: monthly **$4 plus $2 per domain**. And you can deploy with one command: `bundle exec middleman fjords --rebuild`
