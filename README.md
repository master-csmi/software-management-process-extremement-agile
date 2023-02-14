# Presentation on Agile Methodologies

## Building from sources

### Deps

This Asciidoctor depends on Ruby and RVM. Hence make sure to have this program on your computer.

Then install Bundler

```bash
gem install bundler
```

### Cloning the repo

Clone and `cd` into this repository.

Then configure Bundler environment

```bash
bundle config --local path .bundle/gems
bundle
```

Cloning revealjs

```bash
git clone -b 3.9.2 --depth 1 https://github.com/hakimel/reveal.js.git
```

### Build Presentation in HTML format

```bash
bundle exec asciidoctor-revealjs index.adoc
```

### Speaker Notes

First run a web server in this folder

```bash
ruby -run -e httpd . -p 5000 -b 127.0.0.1
```

Then open `index.html`

```bash
http://127.0.0.1:5000/index.html
```

and press `s`.
