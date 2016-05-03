<img src="http://i.imgur.com/EohdCC9.png" width="66px">

## Static site enlightenment

Static site prototyping toolkit originally forked from Kriasoft's [Static Site Starter Kit](https://github.com/kriasoft/static-site-starter) and inspired by Thoughtbot's [Proteus](https://github.com/thoughtbot/proteus) kits.

#### Includes

 * [Pug](https://github.com/pugjs/pug): Formerly Jade, happy JS templating.
 * [Gulp](http://gulpjs.com/): Extend using whatever gulp plugins you like.
 * [Sass (LibSass)](http://sass-lang.com):
   CSS with superpowers
 * [Bourbon](http://bourbon.io):
   Sass mixin library
 * [Neat](http://neat.bourbon.io):
   Semantic grid for Sass and Bourbon
 * [Bitters](http://bitters.bourbon.io):
   Scaffold styles, variables and structure for Bourbon projects.
 * [BrowserSync](http://www.browsersync.io): Test your prototype across multiple devices with Buddha-like power.

#### Why?

I really like Proteus, particularly the Middleman kit, but I got sick of Ruby's weirdness. I wanted a JS-based solution for quickly spinning up static sites and prototyping without having to wrangle with weird plugins and cryptic errors from Ruby gems.

## Todo

* Frontmatter compatibility
* Helper functions
* Possibly a CLI of some sort
* And a bunch else I haven't thought of yet, I'm sure


## Getting Started

 1. [Fork](https://github.com/steviant/zazen/fork) or [download](https://github.com/Steviant/zazen/archive/master.zip) this repo.
 2. Open the directory in your terminal and enter:
 ```sh
 $ npm install
 ```

#### Questions & Answers

* [How to deploy the site to GitHub Pages?](./docs/faq.md#how-to-deploy-the-site-to-github-pages)
* [How to deploy the site via SCP?](./docs/faq.md#how-to-deploy-the-site-via-scp)
* [How to securely store sensitive data in my public repository?](./docs/faq.md#how-to-securely-store-sensitive-data-in-my-public-repo)
* [Read more...](./docs/faq.md)

#### How to Build

```sh
$ gulp build    # or `gulp build --release`
```

#### How to Run

```sh
$ gulp          # or `gulp --release`
```

This command builds the project, launches [BrowserSync](http://www.browsersync.io)
development server and starts listening for modifications in source files.

#### How to Deploy

If [Travis CI](https://travis-ci.org/) is watching this repo, it will deploy
the site automatically after each commit. Otherwise, you may deploy it manually
by running:

```sh
$ gulp deploy   # or `gulp deploy --production`
```

You just need to make sure that you have set [GITHUB_TOKEN](https://github.com/settings/applications) environment variable.

#### Keeping Up-to-Date

Down the road you may want to pull and merge the latest updates from this repo
back to your local project. To do so, you simply run:

```sh
$ git fetch upstream
$ git checkout master
$ git merge upstream/master
```

For more details see: [Syncing a Fork on GitHub](https://help.github.com/articles/syncing-a-fork)

#### Contributors

 - Steve Mitchell -- [@steviant](https://github.com/steviant)
 - Konstantin Tarkus -- [@koistya](https://twitter.com/koistya)
 - Vladimir Kutepov -- [@frenzzy](https://github.com/frenzzy)
