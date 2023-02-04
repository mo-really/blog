# blog

1. [Install Hugo](https://github.com/gohugoio/hugo#fetch-from-github)

```bash
CGO_ENABLED=1 go install --tags extended github.com/gohugoio/hugo@latest
```

2. [Make it a hugo site](https://gohugo.io/getting-started/quick-start/)

```bash
hugo new site . --force
```

3. [Add the theme](https://themes.gohugo.io/)

```
git submodule add https://github.com/theNewDynamic/gohugo-theme-ananke themes/ananke
```

4. Add theme to config.toml

```
echo "theme = 'ananke'" >> config.toml
```

5. Serve the site

```
hugo server -D --baseUrl="/" --appendPort=false
```