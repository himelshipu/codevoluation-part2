<template>
  <div >
    <h3> {{title}} </h3>
    <p v-bind="$attrs">
      Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy
      text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book. It has survived not
      only five centuries, but also the leap into electronic typesetting, remaining essentially unchanged. It was popularised in the 1960s with
      the release of Letraset sheets containing Lorem Ipsum passages, and more recently withdesktop publishing software like Aldus PageMaker
      including versions of Lorem Ipsum.
    </p>
    <h5> {{likes}} - People Appriciated </h5>
    <h5>Publishing Status - {{isPublished ? 'published Already' : 'Not Published Yet'}}  </h5>
  </div>


</template>
<script>
export default {
  name:'Article',
  props:{
    title:{
      type: String,
      default: 'show this if any title not found' ,
      required: true,
    },
    likes:Number,
    isPublished: Boolean,
  },
  inheritAttrs: false,
}

</script>

<style>

</style>