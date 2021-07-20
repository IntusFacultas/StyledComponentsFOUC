<template>
  <div>
    <StyledTitle>FOUC?</StyledTitle>
    <Tutorial/>
  </div>
</template>

<script>
import styled, { StyleSheet, ServerSideRenderMixin } from 'vue-styled-components';
StyleSheet.serverRendered = true

const StyledTitle = styled.h1`
  font-size: 35px;
  color: red;
  font-family: sans-serif;
  font-weight: bold;
`
export default {
  components: {
    StyledTitle
  },
  mixins: [ServerSideRenderMixin],
}
</script>
