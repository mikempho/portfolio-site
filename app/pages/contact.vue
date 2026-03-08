<template>
  <h1>Contact Me</h1>
  <!-- <h2>Contact Form</h2> -->
  <form name="contact" method="POST" data-netlify="true">
    <input type="hidden" name="form-name" value="contact">
    
    <label name="name">Name </label>
    <input type="text" name="name" required/>

    <label>Email </label>
    <input type="email" name="email" required/>

    <label>Message </label>
    <textarea name="message" required></textarea>

    <button type="submit">Send</button>
  </form>
  
</template>

<script>

</script>

<style scoped>
  h1{
    text-align:center;
    padding:20px;
  }

  form {
    padding-top:30px;
    max-width:500px;
    margin:auto;
    display:flex;
    flex-direction:column;
    gap:15px;
  }

  label {
    padding: 0px 15px;
  }

  input {
    border-radius: 6px;
    border:none;
    padding: 10px;
  }

  textarea {
    min-height:120px;
    border-radius: 6px;
  }

  form button {
    padding:10px;
    background-color:#e9c46a;
    border:none;
    border-radius:6px;
    cursor:pointer;
  }

  form button:hover {
    background-color:#d1ab4c;
  }

</style>