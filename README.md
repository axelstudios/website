## BuildingSync Jekyll Site

## How to use it
### Running locally
`jekyll serve`



### Deployment

**Important:**  For security reasons, Github doesn't allow plugins (under _plugins/) when deploying with Github Pages. This means:

**1)** that we need to generate your site locally (more details below) and push the resulting HTML to a Github repository;

**2)** built the site with [travis-ci](https://travis-ci.org/) (with goodies from [jekyll-travis](https://github.com/mfenner/jekyll-travis)) automatically pushing the generated *_site/* files to your *gh-pages* branch.
 This later approach is the one I am currently using to generate the live demo.

For option **1)** simply clone this repository (*master branch*), and then run `jekyll serve` inside the directory. Upload the resulting *_site/* contents to your repository (*master branch* if uploading as your personal page (username.github.io) or *gh-pages branch* if uploading as a project page (as for the [demo](https://github.com/biomadeira/jasper/tree/gh-pages)).

For option **2)** you will need to set up travis-ci for your personal fork. Briefly all you need then is to change your details in *[\_config.yml](_config.yml)* so that you can push to your github repo. You will also need to generate a secure key to add to your *[.travis.yml](.travis.yml)* (you can find more info on how to do it in that file). Also make sure you read the documentation from [jekyll-travis](https://github.com/mfenner/jekyll-travis). This approach has clear advantages in that you simply push changes to your files and all the html files are generated for you. Also you get to know if everything is still fine with your site builds. Don't hesitate to contact me if you still have any issues (see below about issue tracking).

## Copyright & License

Copyright (C) 2015 - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

