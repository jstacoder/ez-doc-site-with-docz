
### Heres how to make an easy site with docz

---

### Create a directory

```bash
$ mkdir my-project-docs
$ cd my-project-docs
```

but call it whatever you want.

### Install Dependencies

```bash
$ yarn init -y
$ yarn add react react-dom gatsby gatsby-theme-docz@next docz@next
```

Now we only need to add 2 small files and were done:

1. `gatsby-config.js` - a configuration file, this is where we tell 
`gatsby` to use `docz`

2. some mdx file, we will start with our index/getting statrted page

`gatsby-config.js`
```js
module.exports = {
  plugins: [
    `gatsby-theme-docz`
  ]
}
```

`src/pages/index.mdx`
```mdx
---
  name: Getting Started
  route: /
  menu: 
---

## Here is our first doc page
```

Thats all you need, now you can check out your new website with: 

```bash
$ gatsby develop
```

Go ahead see...
