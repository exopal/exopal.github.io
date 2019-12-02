

## Important
> Only use Github client to interract with Exopal documentation

## Be aware of OSX Mojave
On OSX mojave some ruby header are locked by the system, you need to install ruby 2.6.2 (jekyll compatible). Then  you can run bundle insall.

## Based on

This production documentation site is based on 

[View the documentation](https://pmarsceill.github.io/just-the-docs/) for usage information.

## Getting started

Clone [Github repositoryremote theme](https://github.com/exopal/exopal.github.io.git)

### Local installation: Use the gem-based theme

1. Install dependencies
```bash
$ `bundle install`.
```
2. _Optional:_ Initialize search data (creates `search-data.json`)
```bash
$ bundle exec just-the-docs rake search:init
```
3. Run you local Jekyll server
```bash
$ jekyll serve
```
```bash
# .. or if you're using a Gemfile (bundler)
$ bundle exec jekyll serve. (RUN COMMAND)
```
4. Point your web browser to [http://localhost:4000](http://localhost:4000)

If you're hosting your site on GitHub Pages, [set up GitHub Pages and Jekyll locally](https://help.github.com/en/articles/setting-up-your-github-pages-site-locally-with-jekyll) so that you can more easily work in your development environment.

### Configure Just the Docs

- [See configuration options]({{ site.baseurl }}{% link docs/configuration.md %})

## About the project

Exopal documentation jekyll based on Just the Docs is &copy; 2017-2019 by [Patrick Marsceill](http://patrickmarsceill.com).


## License

Just the Docs is distributed by an [MIT license](https://github.com/pmarsceill/just-the-docs/tree/master/LICENSE.txt).

The theme is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).
