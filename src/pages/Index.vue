<template>
  <q-page class="flex flex-center">
    <div class="q-gutter-lg " style="max-width: 300px">
      <q-btn icon="mail" padding="lg" color="primary" text-color="white" label="TypePage" @click="gotoPage('/type')"/>
      <q-btn icon="mail" padding="lg" color="primary" text-color="white" label="TestPage" @click="gotoPage('/test')"/>
      <!-- <q-input v-model="text" label="standard" outlined mask="NNN-NNN-NNNN"/>
      <q-radio v-model="shape" val="line" label="선" />
      <q-radio v-model="shape" val="rectangle" label="사각형" />
      <q-radio v-model="shape" val="ellipse" label="타원" />
      <q-radio v-model="shape" val="polygon" label="다각형" />
      <q-checkbox v-model="right" label="면 추가" /> -->
    </div>
  </q-page>
</template>

<script>
export default {
  name: 'PageIndex',
  data() {
    return {
      text : 'ym',
      shape: 'line',
      right : false,
    }
  },
  methods : {
    gotoPage(url) {
      this.$router.push(url);
    }
  }
}
</script>
