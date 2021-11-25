<template>
  <h1>random</h1>
  <center><p>{{ message }}</p></center>
  <center><button @click="random">math random number</button></center>
  <h1>random </h1>
  <center><p>{{ msg }}</p></center>
  <center><button @click="rando">random phrase or word</button></center>
</template>

<script>
export default {
  data() {
    return {
      message: 'click in the button for math random number',
      msg: 'click in the button for random phrase or word'
    }
  },
  methods: {
    random() {
      this.message = Math.random()
    },
    rando() {
        const f = [
            'hello', 
            'bye', 
            'octuber', 
            'offline', 
            'online', 
            'cat', 
            'dog', 
            'hi', 
            'github', 
            'javascript', 
            'ruby', 
            'csharp', 
            'wow', 
            'fuck', 
            'pineapple', 
            'apple', 
            'otter', 
            'follow',
            'commit', 
            'think', 
            'beautiful', 
            'js',
            'topic',
            'book', 
            'info', 
            'chat', 
            'array', 
            'condition',
            'hey', 'who',
            'asked', 
            'why',
            'what'];
const r = Math.floor(Math.random() * f.length);
this.msg = f[r];
    }
  }
}
</script>