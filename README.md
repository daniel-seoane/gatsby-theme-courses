⚠️ Warning! ⚠️

This repository hasn't been maintained in a long time.


# Courses Theme

A minimalist Gatsby theme for creating courses

Check out the [live demo](https://gatsby-theme-courses-demo.netlify.com)

## ✨Features

- Minimalist and fast
- Create courses and lessons with MDX
- Multiple video hosts: Youtube, Facebook, Vimeo, Wistia, Twitch and [more](https://github.com/CookPete/react-player#supported-media) 
- Styling with Theme UI
- Responsive

## 🚀Installation

1. Install the theme

```sh
npm install --save gatsby-theme-courses
```

or

```sh
yarn add gatsby-theme-courses
```

2. Add the theme to your `gatsby-config.js`

```javascript
// gatsby-config.js
module.exports = {
  plugins: [
    {
      resolve: 'gatsby-theme-courses',
      options: {
        // See config section for more information
      },
    },
  ],
}
```

## 📝Config

| Key                      | Default value     | Description                                                       |
| ------------------------ | ----------------- | ----------------------------------------------------------------- |
| `basePath`               | `/`               | Root url for all courses                                          |
| `coursesPath`            | `content/courses` | Location of courses                                               |
| `authorsPath`            | `content/authors` | Location of authors                                               |
| `mdxOtherwiseConfigured` | `false`           | Set this flag `true` if `gatsby-plugin-mdx` is already configured |

## 📚Example

### Course definition

`courses/become-react-developer/index.mdx`

```yml
---
title: Become a React Developer
description: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut eleifend nibh vel blandit interdum
author: John Doe
cover: ./assets/cover.png
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit.
```

### Lessons

`courses/become-react-developer/hello-world.mdx`

```yml
---
title: Hello World
description: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut eleifend nibh vel blandit interdum.
duration: "9:28"
number: 1
video: https://www.youtube.com/embed/dQw4w9WgXcQ
---

Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut eleifend nibh vel blandit interdum.
```

### Authors

`authors/authors.yml`

```yml
- name: John Doe
  bio: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut eleifend nibh vel blandit interdum. Phasellus vel sodales justo, vel maximus tellus.
  avatar: ./avatars/john-doe.webp
  link: https://example.com
```

## 👥Shadowing

You can customize the theme using shadowing

[Shadowing in Gatsby Themes](https://www.gatsbyjs.org/docs/themes/shadowing/)

## License

[MIT](LICENSE)
