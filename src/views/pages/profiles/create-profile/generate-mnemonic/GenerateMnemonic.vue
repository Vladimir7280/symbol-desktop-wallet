<template>
  <div class="step-2-wrapper" @mouseover="shouldTrackMouse && handleMousemove($event)">
    <img src="@/views/resources/img/back.png" />
    <div class="progress-bar">
      {{ $t('move_your_mouse') }}
    </div>
    <Progress :stroke-width="20" stroke-color="#6401ee" :percent="percent" />
  </div>
</template>

<script lang="ts">
import GenerateMnemonicTs from './GenerateMnemonicTs'
export default class GenerateMnemonic extends GenerateMnemonicTs {}
</script>
<style lang="less" scoped>
@import './GenerateMnemonic.less';
</style>
