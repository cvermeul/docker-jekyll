# How to use this image

#### Create new project

    docker run -v "$PWD:/src" cvermeul/jekyll new myproject
  
#### Build ...
    cd myproject
    docker run -v "$PWD:/src" cvermeul/jekyll build

#### ... or Serve
    docker run --rm -v "$PWD:/src" -p 4000:4000 cvermeul/jekyll serve -H 0.0.0.0

##### With `--watch` option

    docker run --rm -v "$PWD:/src" -p 4000:4000 cvermeul/jekyll serve --watch --force_polling -H 0.0.0.0
