# Hugo Modules

## Sample Site Banner

Add the following code to your module list in the config/_default/module.toml file.

``` toml
[[imports]]
    path = "github.com/davefass/hugo-modules"
```

Or in hugo.toml file

``` toml
[module]
  [[module.imports]]
    path = 'github.com/davefass/hugo-modules'
```

Call it as a partial in your baseof.html file above the header partial.

``` hugo
{{ partialCached "banner.html" . }}
```
