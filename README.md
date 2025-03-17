# Hugo Modules

1. init current project as module

``` zsh
hugo mod init github.com/user/current-project
```

2. add code below to indicated files in current project
3. pull modules into current project

``` zsh
hugo mod get -u
``` 

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

``` go
{{ partialCached "banner.html" . }}
```
