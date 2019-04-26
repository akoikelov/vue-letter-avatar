<template>
<div>
  <span v-for='letter of allLetter'>
    <vue-letter-avatar class='letter-avatar' :name='letter' :rounded=true />
  </span>
  <vue-letter-avatar class='letter-avatar' :name='complex_text' :rounded=true />
  <vue-letter-avatar class='letter-avatar' :name='empty_text' :rounded=true />
  <vue-letter-avatar class='letter-avatar' :name='single_word_text' :rounded=true />
</div>
</template>
<style scope>
.letter-avatar {
  margin: 10px;
}
</style>
<script>
export default {
  data() {
    return {
      allLetter: 'abcdefghijklmnopqrstuvwxyz',
      complex_text: 'Adam Sandler',
      empty_text: '',
      single_word_text: 'Adam',
    };
  }
};
</script>
