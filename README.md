# nuxt-vuetify-module-bug

> Sample project to reproduce a bug with the Nuxt vuetify-module

## Build Setup

``` bash
# install dependencies
$ npm run install
```

## Steps to reproduce bug

1. Start the Nuxt app
```bash
$ npm run dev
```
2. Open the app in a browser and notice the custom header that is present
3. Open `nuxt.config.js` in your editor of choice and change `treeShake` to true (line 40)
4. Wait for the Nuxt app to rebuild and then refresh the browser
5. Notice how the custom header no longer appears. If you use the element inspector in Chome, you will see that the `v-app-bar` element appears verbatim and is never transpiled.
