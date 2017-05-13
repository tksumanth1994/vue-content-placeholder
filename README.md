# vue-content-placeholder

Inspired by [Facebook content placeholder deconstruction](http://cloudcannon.com/deconstructions/2014/11/15/facebook-content-placeholder-deconstruction.html)

## Get stared

Here is [DEMO](https://stevenyuysy.github.io/vue-content-placeholder/).

![](demo.gif)

## How it work?

You can check out the article above. The difference is that I use the property of `flex` instead of `absolute` in every row.

The boxes can be custom height and custom width, you can choose a fixed height with `px`, or just use Number to declare its `flex-basis` or use `%`, `em` ...

### Import

#### ES6

```js
/* in xxx.vue */

import ContentPlacehlder from 'vue-content-placeholder/dist/ContentPlaceholder.vue'

export default {
  ...
  components: {
    ContentPlaceholder
  },
  ...
}
```

#### ES5

```js
var Vue = require('vue')
var ContentPlacehlder = require('vue-content-placehlder')

var YourComponent = Vue.extend({
  ...
  components: {
    'content-placehlder': ContentPlacehlder.default
  },
  ...
})
```

## Option

| Options | type | discription|
| -- | -- | -- |
| rows | Array  | The property of the component |
| row  | Object | The element of the rows |
| row.height | String | The height of the row, support `px`, `rem`, `em`, `%` |
| row.boxes | Array | The transition boxes of the row |
| box | Array | The box in the row.boxes |
| box[0] | String `||` Number | To declare the width of the left gutter |
| box[1] | String `||` Number | To declare the width of the box |


## Contribution

- Fork it
- PR
