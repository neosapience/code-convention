# Frontend Code Convention
> [vue style guide](https://vuejs.org/v2/style-guide/#Prop-definitions-essential)

## Rules:
* vue style guide, strong recommended
* spacing: 2, no tab
* semicolon: no semi
* quatation mark:
  * template: double quotation, backtick
  * script: single quotation, backtick
  * css: double quotation
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
        'ccc': 'ddd'
      }
    }
  }

  for (let i = 0; i < 10; i++) {
    console.log('success')
  }
}).catch(error => {
  console.log('error')
})
```

```vue
<template>
  <div>
    <h1>{{ data }}</h1>
    <h2 :style="{a: 'bb', c:'cc'}"></h1>
  </div>
</template>
```

## tools
Vetur + es-lint + prettier
