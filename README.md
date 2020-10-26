# webpack5-persistent-cache

### Tested on:
* `node: v12.18.3`
* `npm: 6.14.6`

### Steps to reproduce:

* `npm install`
* change the `fullPath` variable in the `webpack.config.js`
* `npm run build`
* `npm run serve`
* go to `localhost:8080`
  * You should see the text: 'Just a text'.
* edit the file in `src/App.jsx`
  * just change the text 'Just a text' to something else.
  * Save.
* run `npm run build` again
* refresh `localhost:8080`

The text left unchanged - it's cached result even though source has changed.
