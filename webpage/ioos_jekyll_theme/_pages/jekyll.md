---
layout: single
excerpt: "Jekyll Setup"
sitemap: false
permalink: /pages/jekyll/
---
## Jekyll Setup ##
This is just a placeholder page with Markdown examples describing the Jekyll/
Minimal Mistakes theme setup used in this site.

### Requirements: ###
- Ruby: [https://www.ruby-lang.org/en/](https://www.ruby-lang.org/en/), Windows users:
  [Ruby Installer for Windows](http://rubyinstaller.org/downloads/)
- Jekyll: [https://jekyllrb.com/](https://jekyllrb.com/)
- Minimal Mistakes Jekyll theme: [https://mmistakes.github.io/minimal-mistakes/](https://mmistakes.github.io/minimal-mistakes/)

*\*Minimal Mistakes theme was the base theme used for the site*


### Installation: ###
- Install Ruby for your environment (via package manager(unix) or installer (win))

- Install Jekyll in your Ruby environment:

```
gem install jekyll
```

- The Minimal Mistakes theme docs recommend installing Bundler for dependency
management to run Jekyll.  See the [install docs](https://mmistakes.github.io/minimal-mistakes/docs/installation/)
for more info.

```
gem install bundler
```

- Checkout the GitHub repo to get the code:

```
cd /my/sourcecode/dir
git clone https://github.com/ioos/ioos_jekyll_theme.git
cd catalog
```

- Install dependencies via Bundler:

```
bundle install
```


- From here, you should be able to run Jekyll to preview the site as follows:

```
bundle exec jekyll serve --config _config.yml,_config_dev.yml
bundle exec jekyll serve --config _config.yml,_config_dev.yml --watch --verbose
bundle exec jekyll serve --config _config.yml,_config_dev.yml --watch --verbose --incremental
```

Note: the --config flag allows local overrides of the site.url for development/testing
in the \_config_dev.yml file, while the production version when pushed to GitHub will use the settings in
the standard Jekyll \_config.yml file only.
