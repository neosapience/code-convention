# Frontend Code Convention
> [vue style guide](https://vuejs.org/v2/style-guide/#Prop-definitions-essential)

## Installation

### Requirement

- vscode
  - extensions
    - eslint
    - prettier
    - vetur

### How To Setting

1. run vscode, install eslint, prettier, vetur extension
2. open setting (`cmd + ,`)
3. find `format javascript`. unchecked item
![format javascript setting](screenshot/setting_1.png 'Import')
3. find `format on save`. check item
![format javascript setting](screenshot/setting_2.png 'Import')

## Rules:
* vue style guide, strong recommended
* spacing: 2, no tab
* semicolon: no semi
* quatation mark:
  * template: double quotation, backtick
  * script: single quotation, backtick
  * css: double quotation
* print width: 200
* bracket spacing: false
```js
/* BAD */
const data = { key: 'value' } 

/* GOOD */
const data = {key: 'value'}
```
* no `var`, recommended `let`
* filename:
  * scss, css -> underscore, `-`
  * export class: Pascal case
  * export object or function: Camel case.
* trailing comma
```js
let aa = [
  'aaa',
  'bbb',
]

const bb = {
  first: {
    ...
  },
  second: {
    ...
  },
}
```

* function
```js
export default {
  data (aaa, bbb) {
    return {
      foo: 'bar'
    }
  }
}

func2(data, {app: $axios}).then(res => {  
  let data2 = {
    'aaa': {
      'bbb': {
        'ccc': 'ddd',
      },
    },
  }

  for (let i = 0; i < 10; i++) {
    console.log('success')
  }
}).catch(error => {
  console.log('error')
})
```

```html
<template>
  <div>
    <h1>{{ data }}</h1>
    <h2 :style="{a: 'bb', c:'cc'}"></h1>
  </div>
</template>
```

## tools
Vetur + es-lint + prettier
