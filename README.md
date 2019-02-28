# port-folio-site
designed by MohanaPragada

This is the source code to my personal blog and website.

This website was one of my first forays into building a full website using NodeJS. I chose this runtime rather than one which I'm more comfortable with because it gives me the opportunity to learn something new. Besides, Node is a lot of fun to work with. Please note that the code written here isn't perfect. Copy at your own risk!

## How it's built

### Data

A majority of the website's page content is stored in the `/data/` directory in HTML or MD files. I started with HTML but soon decided that Markdown would be more future proof as it could easily be ported between websites without much work. Further more, it allows the viewing of the content on GitHub in a pretty way.

This file defines that if the website is visited at `/blog/`, then a page will be returned using the `blogs` controller.

This approach of storing the data in JSON files in a file structure means that for now I can avoid using a database (and all of the overhead that comes with that, including development/staging/live databases and backing them up).

The benefits of this approach include that the JSON files can simply be indexed into a Mongo-like database in the future.

### Views

Views are built using EJS. It's not the most pretty but it works on the front end or back end so there's no need to learn two templating engines when I can just learn one. They're all basically the same anyway, right?

### Sass/CSS

SCSS is used to style the website. Susy is used as the grid system to give me full control of the website.
