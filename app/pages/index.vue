<template>
  <div class="hero-section">
    <div class="left-header">
      <p>Hello, <span class="name">I'm Mike Matseane</span></p>
      <h1>Aspiring Multimedia Specialist <span v-if="emoji" v-html="emoji.htmlCode[0]" class="emoji"></span></h1>
      <p>I am a BIS Multimedia student with a passion for technology, digital media, and creative problem-solving. My interests include web development, software design, and multimedia production. I enjoy building interactive applications and exploring how technology can be used to create engaging digital experiences.</p>
    </div>
    <div class="right-header">
      <img src="/images/profile.jpg" width="200">
    </div>
  </div>

  <div class="quote-box" v-if="quoteData">
    <h2>Qoute of the Day</h2>
    <p>"{{ quoteData.quoteText }}"</p>
    <p class="quoteAuthor">"{{ quoteData.quoteAuthor }}"</p>
  </div>

  <p v-else-if="error">Failed to load quote</p>
</template>

<script setup>
  const {data: quoteData, error } = await useFetch("https://api.forismatic.com/api/1.0/?method=getQuote&format=json&lang=en");

  const {data: emoji} = await useFetch("https://emojihub.yurace.pro/api/random");
</script>

<style scoped>
  .hero-section {
    display:flex;
    justify-content:space-between;
    margin-top:7rem;
    align-items:center;
  }

  .hero-section div {
    margin: 0px 50px;
  }

  .right-header img {
    border-radius: 20px;
  }

  .name{
    color:#e9c46a;
  }

  .quote-box {
    max-width:400px;
    background-color:aliceblue;
    padding: 20px;
    color:black;
    margin: 50px 50px;
    border-radius: 20px;
  }

  .quoteAuthor {
    margin-left:20px;
  }

  .emoji {
    font-size: 30px;
  }
</style>