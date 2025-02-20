# 快捷选项

你可以自定义一些快捷按钮.

```html
<n-space vertical>
  <n-date-picker v-model:value="ts1" type="date" :shortcuts="shortcuts" />
  <n-date-picker v-model:value="ts2" type="datetime" :shortcuts="shortcuts" />
  <n-date-picker
    v-model:value="range1"
    type="daterange"
    :shortcuts="rangeShortcuts"
  />
  <n-date-picker
    v-model:value="range2"
    type="datetimerange"
    :shortcuts="rangeShortcuts"
  />
</n-space>
```

```js
import { defineComponent, ref } from 'vue'

export default defineComponent({
  setup () {
    return {
      ts1: ref(null),
      ts2: ref(1183135260000),
      range1: ref(null),
      range2: ref(null),
      shortcuts: {
        亲爱的生日: 1631203200000,
        派对日: 1629216000000
      },
      rangeShortcuts: {
        快乐假期: [1629216000000, 1631203200000]
      }
    }
  }
})
```
