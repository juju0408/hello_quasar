<template>
  <q-page padding>
    <h1>TypePage</h1>
    <q-input v-model="text" label="filled" />
    <div class="bg-blue-9 text-white">{{text}}</div>
    <div>{{text.length}}</div>
    <div>{{text + text}}</div>
    <div>{{text.replace("-", "")}}</div>
    <div class="bg-grey">{{text.substr(0, 3) + text.substr(4, 4) + text.substr(9, 4)}}</div>
    <div>{{text.includes('abc')}}</div>
    <div>{{text.replace('슈발놈', '**놈').replace('착한놈', '**놈')}}</div>
    <div>{{number % 2 == 0}}</div>
  </q-page>
</template>

<script>
export default {
  // name: 'PageName',
  data() {
    return {
      // text : '0123456789',
      text : '010-3448-1833',
      number : 4,
    }
  }
}
</script>
