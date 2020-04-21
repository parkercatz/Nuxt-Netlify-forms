<template>
  <section class="section">
    <div class="inner">
      <h2 class="title">
        CONTACT
      </h2>
      <p class="subtitle">
        お問い合わせ
      </p>
      <div class="tab">
        <button
          v-for="tab in tabs"
          :key="tab.id"
          :class="['button', { active: selected === tab.label }]"
          @click="selected = tab.label"
        >
          {{ tab.content }}
        </button>
      </div>
      <div class="contents">
        <component :is="selected" />
      </div>
    </div>
  </section>
</template>

<script>
import Form01 from '~/components/Form01'
import Form02 from '~/components/Form02'

export default {
  components: {
    Form01,
    Form02
  },
  data() {
    return {
      tabs: [
        { id: 1, label: 'Form01', content: '個人の方' },
        { id: 2, label: 'Form02', content: '企業の方' }
      ],
      selected: 'Form01'
    }
  }
}
</script>
<style>
.tab {
  margin-bottom: 2em;
}
</style>
