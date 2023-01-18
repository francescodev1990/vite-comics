<script lang="ts">
export default {
  data() {
    return {
      link: [
        {
          titolo: "DC COMICS",
          link: [
            "Personaggi",
            "Cartoni",
            "Film",
            "TV",
            "Giochi",
            "Video",
            "News",
          ],
        },
        {
          titolo: "SHOP",
          link: ["Shop DC", "Shop DC Collezionabili"],
        },
        {
          titolo: "DC",
          link: [
            "Termini di utilizzo",
            "Privacy Policy",
            "Aggiungi Scelta",
            "Advertising",
            "Lavoro",
            "Sottoscrizioni",
            "Talent Workshops",
            "CPSC Certificates",
            "Classifica",
            "Shop FAQ",
            "Contatti",
          ],
        },
        {
          titolo: "SITES",
          link: [
            "DC",
            "MAD Magazine",
            "DC Kids",
            "DC Universe",
            "DC Power Visa",
          ],
        },
      ],
    };
  },
};
</script>
<template lang="">
    <footer>
        <div class="footer_content">
        <div class="container">
            <div v-for="(item, index) in link" :key="index">
                {{item.titolo}}
                <ul>
                    <li v-for="(item, index) in link" :key="index">
                        {{item.link}}

                    </li>
                </ul>
                

            </div>
        </div>
    </div>
    </footer>
    
</template>

<style lang="scss" scoped>
.footer_content {
  background-image: url(../assets/images/footer-bg.jpg);
  background-size: cover;
}
</style>