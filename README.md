## landingpage-executive


This is the executive version of the cookbook landingpage.

Designed to make a mid-level manager interested in the cookbook, and delegate the in-depth tasks to her/his team.


## where lives the content

The content lives in `/data` directory, and is stored as json. No idea how HTML / markdown formatting is possible in json, as of now.


## learning more about available options for the content

Unfortunately, the template is not officially documented. You can look up possible options for the content in the directory `themes/hugo-lime/layouts/`, particularly in the `partials` directory there. 
(!! NOT YET WORKING: visit at <https://fairplus.github.io/landingpage> !!)


## Using Lime Theme Starter
This page is based on [hugo-lime](https://themes.gohugo.io/hugo-lime/).

## local development

```
git clone --recurse-submodules https://github.com/FAIRplus/landingpage-executive.git
cd landingpage-executive
docker run --rm -it -v $(pwd):/src -p 1313:1313 klakegg/hugo:0.73.0-ext-alpine server
``` 

The docker will continue running. You can stop the server by pressing Ctrl + C (but obviously, the server and the page will be dead, then).

Visit <http://localhost:1313> to see the page live (the docker container has to be running).

## hugo docker 

available from: https://hub.docker.com/r/klakegg/hugo/

## hugo CI/CD

available from: https://github.com/peaceiris/actions-hugo