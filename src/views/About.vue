<template>
  <div id="wrap" class="light">
    <Header />
    <Layout />
    <!-- about -->
    <section id="aboutCont">
      <div class="container">
        <h2>ABOUT ME</h2>
        <div class="about-cont">
          <div class="about">
            <div class="about-img">
              <div v-for="todo in todos" v-bind:key="todo.text">
                {{ todo.text }}
                <div class="about-txt">
                  <div v-for="todo in todos" v-bind:key="todo.text">
                    {{ todo.text }}
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- //about -->
  </div>
</template>
<script>
import Header from "@/components/Header.vue";
export default {
  components: {
    Header,
  },
  data: function () {
    return {
      todos: [
        { text: "we provide" },
        { text: "visual coding" },
        { text: "solutions" },
        { text: "for you webs" },
      ],
    };
  },
};
</script>
