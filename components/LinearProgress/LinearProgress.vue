<template>
    <div role="progressbar" class="mdc-linear-progress">
        <div class="mdc-linear-progress__buffering-dots"></div>
        <div class="mdc-linear-progress__buffer"></div>
        <div class="mdc-linear-progress__bar mdc-linear-progress__primary-bar">
            <span class="mdc-linear-progress__bar-inner"></span>
        </div>
        <div class="mdc-linear-progress__bar mdc-linear-progress__secondary-bar">
            <span class="mdc-linear-progress__bar-inner"></span>
        </div>
    </div>
</template>

<script>
import { MDCLinearProgress } from '@material/linear-progress'

export default {
  props: {
    open: {
      type: Boolean,
      required: false
    },
    indeterminate: {
      type: Boolean,
      required: false
    },
    reverse: {
      type: Boolean,
      required: false
    },
    progress: {
      type: Number,
      validator: (value) => (value >= 0) && (value <= 1),
      required: false
    },
    buffer: {
      type: Number,
      validator: (value) => (value >= 0) && (value <= 1),
      required: false
    }
  },
  data () {
    return {
      mdcLinearProgress: null
    }
  },
  watch: {
    progress () {
      this.mdcLinearProgress.progress = this.progress
    },
    buffer () {
      this.mdcLinearProgress.buffer = this.buffer
    },
    indeterminate () {
      this.mdcLinearProgress.determinate = !this.indeterminate
    },
    reversed () {
      this.mdcLinearProgress.reverse = this.reversed
    },
    open () {
      this.open ? this.mdcLinearProgress.open() : this.mdcLinearProgress.close()
    }
  },
  mounted () {
    this.mdcLinearProgress = MDCLinearProgress.attachTo(this.$el)
    this.mdcLinearProgress.determinate = !this.indeterminate
    this.mdcLinearProgress.reverse = this.reverse
    this.mdcLinearProgress.progress = this.progress
    this.mdcLinearProgress.buffer = this.buffer
    this.open ? this.mdcLinearProgress.open() : this.mdcLinearProgress.close()
  },
  beforeDestroy () {
    this.mdcLinearProgress.destroy()
  },
  methods: {
    show () {
      this.mdcLinearProgress.open()
    },
    hide () {
      this.mdcLinearProgress.close()
    }
  }
}
</script>

<style lang="scss">
@import "@material/linear-progress/mdc-linear-progress";
</style>
