# static-site-stack
A handy static site stack utilizing many favorites:

* [Middleman](http://middlemanapp.com/) Fantastic static sites
* [Livereload](http://livereload.com/) Auto browser refresher
* [GroundworkCSS](http://groundwork.sidereel.com/) has an amazing SASS frontend grid
* [Foreman](https://github.com/ddollar/foreman) Easy command line controls
* [thin](http://code.macournoyer.com/thin/) web server
* [Compass](http://compass-style.org/) SASS toolbox

## Setup
```
git clone https://github.com/wardpenney/static-site-stack.git
bundle install
bundle exec foreman start -f Procfile_development
```

## Deploy

* Registrar [DNSimple](https://dnsimple.com/) The best host ever for many reasons is actually pretty cheap also: **$3 for a couple of domains, or $8 for 10.**
* Host [Fjords](http://fjords.cc/) Is a static site host with deployment handy commands for Middleman. It's a steal of a deal: monthly **$4 plus $2 per domain**.
