# Typography DeCal Website
Developed by [Tony Zhao](http://tonyzhao.org)
* Designed with [Bootstrap 4](https://getbootstrap.com/)
* Built with [Jekyll](https://jekyllrb.com/)
* Hosted by [Github Pages](https://pages.github.com/)

## Editing
**DO NOT EDIT ANYTHING IN THE `docs` FOLDER**.
Any edits in this folder is unstable and will be overwritten. 
Instead, only edit the `.md` files in root directory or `_lectures`. 
If layout style changes need to be made, edit the layout files in `_layouts/`.

The only thing required to develop the site is Jekyll, which requires Ruby.

For macOS, this can be done with

```
brew install ruby
gem install bundler jekyll
```

In order to see your changes, run `jekyll serve`. This will create a local server at your computer for you to explore changes.

If you are satisfied with your changes, run the following commands to push to the live website.
```
jekyll build
git add *
git commit -m "your extremely useful commit message"
git push origin master
```

And then wait a minute or two for GitHub Pages to load the changes at [typographydecal.com](http://typographydecal.com).

### Site-wide Properties

Site-wide properties include course information that should be constant throughout the site. These properties can be found in `_config.yml`

```yml
# Site-wide course information
course_listing: CS98/198-94
course_schedule: Thursdays, 7-8:30pm
course_location: 310 Jacobs Hall
course_units: 1 Unit, PNP
course_semester: Fall 2019
```

### Home page
Should have the following properties in the front matter of `index.md`. For editing the schedule, see lecture pages section below
```yaml
---
layout: index
title: Typography
description: This is a UC Berkeley DeCal diving into the foundations and applications of typography. 
---

```

### Lecture pages
These are all contained in the `_lectures` folder. Lectures will be rendered in alphanumeric order, i.e. `1.md` will be ahead of `2.md`. Lecture files are expected to have some basic properties in the front matter. Everything below the front matter will be rendered from markdown to html.

```yaml
---
title: Fundamentals of Typography
date: 2019-09-16
excerpt: This shows up in the front page
---
## This is a header
Lecture material can be written in markdown here.
```

### Contact
Edit markdown files in `_facilitators`

`contact.md` should have the following front matter
```yaml
---
layout: contact
title: ...
description: ...
---
```

Each facilitor file should be have the following front matter.
```yaml
---
name: ...
email: ...
image: ...
site: ...
---
```

### Syllabus
Edit markdown file `info.md` in root directory. Everything below the front matter will be rendered automatically from markdown to html.


```yaml
---
layout: info
title: ...
description: ...
---
```

### Resources
Edit markdown file `resources.md` in root directory. Everything below the front matter will be rendered automatically from markdown to html.


```yaml
---
layout: resources
title: ...
description: ...
---
```