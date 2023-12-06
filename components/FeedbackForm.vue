<template>
  <div class="feedback-form">
    <form
      netlify
      netlify-honeypot
      name="feedback"
      method="POST"
      action="/success"
    >
      <p class="hidden">
        <label>
          Don’t fill this out if you’re human: <input name="bot-field" />
        </label>
      </p>
      <input type="hidden" name="form-name" value="feedback" />
      <label for="voornaam en achternaam">Voornaam en Achternaam</label>
      <input id="voornaam en achternaam" type="text" Voornaam en Achternaam="Voornaam en Achternaam" required />
      <label for="email">Email</label>
      <input id="email" type="email" name="email" required />
      <label for="telefoonnummer">Telefoonnummer</label>
      <input id="telefoonnummer" type="telefoonnummer" name="telefoonnummer" required />
      <button type="verzenden">Verzenden</button>
    </form>
  </div>
</template>

<style scoped>
.feedback-form {
  margin: 40px 40px;
  min-width: 250px;
  width: 45%;
}
input,
textarea,
button {
  font-size: inherit;
  margin: 15px 0;
  padding: 12px 20px;
  width: 100%;
}

button {
  background-color: teal;
  border: 1px solid black;
  color: white;
  width: 50%;
}

.hidden {
  clip: rect(0 0 0 0);
  clip-path: inset(50%);
  height: 1px;
  overflow: hidden;
  position: absolute;
  white-space: nowrap;
  width: 1px;
}
</style>
