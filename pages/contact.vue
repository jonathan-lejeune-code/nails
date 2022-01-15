<template>
  <v-container>
    <h1>Contact</h1>
    <p>Pour toute question vous pouvez nous contacter :</p>
    <h2>Siége social</h2>
    <div class="googlemap">
      <iframe
        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d4757443.296443593!2d-42.54011046490657!3d34.5744150882629!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0xadd28c30ec90d79%3A0x44652457c0696504!2sOc%C3%A9an%20Atlantique%20Nord!5e0!3m2!1sfr!2sfr!4v1641583961508!5m2!1sfr!2sfr"
        width="100%"
        height="450"
        style="border: 0"
        allowfullscreen=""
        loading="lazy"
      ></iframe>
    </div>

    <h2 class="mt-10">Par mail</h2>
    <v-btn
      color="#f48fb1"
      class="mr-4 mt-5 white--text"
      href="mailto:?subject=Question du site"
      >Envoyé un mail</v-btn
    >
    <h2 class="mt-10">Par téléphone</h2>
    <p>01-02-02-02-02</p>
  </v-container>
</template>

<script>
export default {
  name: 'ContactPage',
}
</script>

<style></style>
