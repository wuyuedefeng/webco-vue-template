<template>
  <div style="padding-top: 20px">
    <div>
      <vm-button @click="hi(0)">default</vm-button>
      <vm-button type="plain" @click="hi(0.5)">plain</vm-button>
      <vm-button type="danger" @click="hi(1)">danger</vm-button>
      <vm-button type="primary" @click="hi(2)">primary</vm-button>
      <vm-button type="warning" @click="hi(3)">warning</vm-button>
      <vm-button type="hollow" @click="hi(4)">hollow</vm-button>
    </div>
    <div style="margin-top: 20px">
      <vm-button disabled @click="hi(5)">default</vm-button>
      <vm-button type="plain" disabled @click="hi(5.5)">plain</vm-button>
      <vm-button type="danger" disabled @click="hi(6)">danger</vm-button>
      <vm-button type="primary" disabled @click="hi(7)">primary</vm-button>
      <vm-button type="warning" disabled @click="hi(8)">warning</vm-button>
      <vm-button type="hollow" disabled @click="hi(9)">hollow</vm-button>
    </div>
    <div style="margin-top: 20px">
      <vm-button disabled loading icon="icon-loading">default</vm-button>
    </div>
    <div style="margin-top: 20px">
      <vm-button size="large" style="display: block; margin-bottom: 20px">default(默认)</vm-button>
      <vm-button style="display: block; margin-bottom: 20px">default(默认)</vm-button>
      <vm-button size="small" style="display: block; margin-bottom: 20px">default(默认)</vm-button>
      <vm-button size="mini" style="display: block; margin-bottom: 20px">default(默认)</vm-button>
    </div>

    <div style="margin-top: 20px">
      <vm-button @click="hi(0)" size="large">large</vm-button>
      <vm-button type="warning" disabled @click="hi(8)">normal</vm-button>
      <vm-button type="danger" size="small" @click="hi(1)">small</vm-button>
      <vm-button type="primary" size="mini" @click="hi(2)">mini</vm-button>
    </div>
  </div>
</template>

<script>
import Button from './Button/button.vue'
export default {
  methods: {
    hi (num) {
      console.log('hi', num)
    }
  },
  components: {
    [Button.name]: Button
  }
}
</script>
