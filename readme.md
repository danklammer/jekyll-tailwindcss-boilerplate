# Jekyll & Tailwind CSS Boilerplate

A bare bones [Jekyll](https://jekyllrb.com/) site which comes preconfigured to use [Tailwind CSS](https://tailwindcss.com/) for styling.

## Features

- 🤍 Ships free of styling or theming. [Add a theme](https://jekyllrb.com/resources/) or [get started with Tailwind CSS](https://tailwindcss.com/docs/utility-first/).
- 📈 Ships Google Analytics and SEO ready
- 🍕 Dev mode: your Jekyll site is refreshed on file changes and all Tailwind CSS classes are available for use.
- 💻 Release mode: CSS is optimised by striping out unused classes and minifying the file.

---

## Install

- [Install Ruby](https://www.ruby-lang.org/en/downloads/)
- [Install NPM](https://www.npmjs.com/get-npm)
- Install Bundler `$ gem install bundler`
- Run `$ npm run setup` to setup the project.

---

## How to Use

### 🍕 Development

```$ npm run dev```

- Generates _all_ Tailwind CSS classes so you can develop without regenerating them.
- Runs the Jekyll watcher which regenerates the site when files are modified.

*Note that the `tailwind.generated.css` file will show changes in git. Ensure to run the release command before committing so that you only commit necessary CSS changes.*

### 💻 Release

```$ npm run rel```

- Generates the minimum Tailwind CSS necessary to display your site in order to keep the file size tiny.
- Minifies the CSS to reduce the file size even more.

To deploy on [Netlify](https://www.netlify.com/) for example, use the following build settings:
- Build command: `npm run build`
- Publish Directory: `_site`