# webco-vue-template

> A Vue.js project

## Build Setup

``` bash
# install dependencies
npm install

# serve with hot reload at localhost:8080
npm run dev
```

For a detailed explanation on how things work, check out the [guide](http://vuejs-templates.github.io/webpack/) and [docs for vue-loader](http://vuejs.github.io/vue-loader).
# webco-vue-template


# Usage

There has a demo at `src/components/Button`

online webco provide base `vars` and `animations` on server same with this project config

if you wanna compile your component  support `px` and `rem`, please write like below
```
font-size: 14px;
// change to 
font-size: pxRem(14)
``` 

server will compile `px` and `rem` two version, `1px = 1rem`
if some one want use `rem` that should config project base on => `1px = 1rem`

### config.json
```
{
  "entry": {
    "button": "button.vue"
  },
  "units": ["px", "rem"]
}
```


# Compile
upload `/src/components/Button/*` files to `webco.cloud` will auto compile `px` and `rem` as your config


---

# Yourself

You can delete Button files and write yours， use this template. 

you can write all your style as your want, and didn't must dependent my config.

please keep all your files in one folder, because upload files don't support folder.
