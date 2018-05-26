EV Website
==========

The Site is created with a static site generator [Jekyll](http://jekyllrb.com/) and hosted on Github.

You can change and add content via the webinterface at Github or download and install it (see [System Preparation](#system-preparation))

A starter project including full setup for Jekyll, GulpJS, SASS, AutoPrefixer &amp; BrowserSync

## Write and change content
### Markdown
This site uses [Markdown](https://guides.github.com/features/mastering-markdown/), a very simple and easy way to write structured content with headlines, paragraphs, images etc.

### Pages and Posts

This site distiguishs between pages for static longterm content (currently only reflected in the topnavigation) and posts for news, announcements and short public notices (shown in different categories on the homepage).

### Change a page
All pages (except homepage) are stored
in the folder `pages`.
There you can open for example the file `about.md` by clicking on the pen-icon (on the right corner at the [file](link to github webview of about.md))  and make your changes after the  so called frontmatter(everything between the `---` at the beginning of the file. please do not change this unless you know what you do)

When you finished your changes please write a short notice in the commit-message form below the file and commit your changes.

### Change a Post

All posts a stored in the `_posts` folder. Changing the post a the same procedure as described in [Change a page](#Change a page)

### Images
#### Picture from the web (flickr, instagram, ...)
Just include into your page/post markdown file:

`![my photo](https://www.twitter.com/imageurl.jpg)`

#### Upload an image and include it into a page or posts
  1. To add an own image to a post or page you have to upload it first. Got to the [` ./assets/`](./assets/) folder and use  the ` upload`-Button on the right top of the editor.

  2. Then go to the page or post markdown file (e.g. `about.md`) and link the path to the image like so: `![title of the image](link-to-the-image)`

  **Example**
  ```Markdown
  ![my photo]({{ site.url }}/assets/my-photo-123.jpg)
  ```  
---
## Advanced Usage

### System Preparation

To use this starter project, you'll need the following things installed on your machine.

1. [Jekyll](http://jekyllrb.com/) - `$ gem install jekyll`
2. [NodeJS](http://nodejs.org) - use the installer or even better [NVM (Node Version Manager)](https://github.com/creationix/nvm).
3. [GulpJS](https://github.com/gulpjs/gulp) - `$ npm install -g gulp` (mac users may need sudo)

Addtionally it's recommended to install [Git](https://git-scm.com/downloads)


## Local Installation

1. Clone this repo, or download it into a directory of your choice.
2. Inside the directory, run `npm install`.

## Usage

**development mode**

This will give you file watching, browser synchronisation, auto-rebuild, CSS injecting etc etc.

```shell
$ gulp
```

**jekyll**

As this is just a Jekyll project, you can use any of the commands listed in their [docs](http://jekyllrb.com/docs/usage/)

---

## Deploy with Gulp (optional)

You can easily deploy your site build to a gh-pages branch. First, follow the instructions at [gulp-gh-pages](https://github.com/rowoot/gulp-gh-pages) to get your branch prepared for the deployment and to install the module. Then, in `gulpfile.js` you'll want to include something like the code below. `gulp.src()` needs to be the path to your final site folder, which by default will be `_site`. If you change the `destination` in your `_config.yml` file, be sure to reflect that in your gulpfile.

```javascript
var deploy = require("gulp-gh-pages");

gulp.task("deploy", ["jekyll-build"], function () {
    return gulp.src("./_site/**/*")
        .pipe(deploy());
});
```

---

## TODO / Improvements
- better sitemap support (priority/images) (x)
- minifiction, uncss, etc (x)
- image optimization (x)
- improve json-ld support for events and albums, tracks (partially done or prepared)(o)
