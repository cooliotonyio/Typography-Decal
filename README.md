# Typography DeCal Website
Developed by [Tony Zhao](http://tonyzhao.org)
* Designed with [Bootstrap 4](https://getbootstrap.com/)
* Built with [Jekyll](https://jekyllrb.com/)
* Hosted by [Github Pages](https://pages.github.com/)

## Editing
**DO NOT EDIT ANYTHING IN `docs` FOLDER**
Any edits in this folder is unstable and will be overwritten. Instead, only edit the `.md` files in root directory or `_lectures`. If layout style changes need to be made, edit the layout files in `_layouts/`.

### Home page
Should have the following properties in the front matter of `index.md`
```yaml
---
layout: index
title: ...
description: ...
course_no: ...
schedule: ...
location: ...
units: ...
---
```

### Contact
Edit markdown files in `_facilitators`

Should have the following front matter
```yaml
---
layout: contact
title: ...
description: ...
---
```

### Course Information
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