<template>
  <div id="wrap">
    <Header />
    <main id="main">
      <!-- mainCont -->
      <section id="mainCont">
        <div class="main__cont">
          <div>{{ msg1 }}</div>
          <div>{{ msg2 }}</div>
          <div>{{ msg3 }}</div>
          <div>{{ msg4 }}</div>
        </div>
      </section>
      <!-- //mainCont -->
    </main>
  </div>
</template>

<script>
import Header from "@/components/Header.vue";

export default {
  components: {
    Header,
  },
  data() {
    return {
      msg1: "WE PROVIDE",
      msg2: "VISUAL CODING",
      msg3: "SOLUTION",
      msg4: "FOR YOU WEBS",
    };
  },
};
</script>
<style lang="scss" scoped>
#mainCont {
  height: 100vh;
  background: #000;
  display: flex;
  justify-content: center;
  align-items: center;

  .main__cont {
    color: #fff;
    font-size: 10vw;
    line-height: 0.85;
    letter-spacing: -0.0275em;
    transition: all 2s;
    text-transform: uppercase;
    font-family: "Saol Display Regular";
  }
}
</style>
