A minimal Alpine-based image for the [Compass](http://compass-style.org/) CSS authoring framework, intended to be a drop-in replacement for running `compass` locally. It makes no assumptions about your configuration or directory structure.

For example:

```
docker run --rm -v $PWD:/src -w /src bhrutledge/compass watch
```

will work if you have  a `config.rb` in the current directory along the lines of:

```
css_dir = "css"
sass_dir = "sass"
images_dir = "img"
javascripts_dir = "js"
```
