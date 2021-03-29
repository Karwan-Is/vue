<template>
  <div class="main-container">
    <div class="banner">
      <img :src="top_banner" alt="banner" />
    </div>

    <h1 class="title">Junior Web Developer In London</h1>
    <h2 class="skills-title">SKILLS</h2>
    <ul class="skills">
      <li class="skill" v-for="skill in skills" v-bind:key="skill.id">
        <img :src="skill.img" />
        <p :class="skill.class_name">{{ skill.title }}</p>
      </li>
    </ul>
  </div>

  <div class="bottom-banner">
    <img :src="bottom_banner" alt="bottom banner" />
  </div>

  <div class="mail">
    <input type="text" placeholder="Email ..." />
    <button>Subscribe</button>
  </div>
</template>

<script>
import top_banner from "../assets/images/top_banner.jpg"
import bottom_banner from "../assets/images/bottom_banner.jpg"
import html from "../assets/images/html.jpg"
import css from "../assets/images/css.jpg"
import js from "../assets/images/js.jpg"
import react from "../assets/images/react.jpg"
import node from "../assets/images/node.jpg"
import mongodb from "../assets/images/mongodb.jpg"
import vue from "../assets/images/vue.jpg"
import angular from "../assets/images/angular.jpg"
export default {
  data() {
    return {
      top_banner: top_banner,
      bottom_banner: bottom_banner,
      skills: [
        {
          id: 1,
          title: "HTML",
          img: html,
          class_name: "html",
        },
        {
          id: 2,
          title: "CSS",
          img: css,
          class_name: "css",
        },
        {
          id: 3,
          title: "JavaScript",
          img: js,
          class_name: "js",
        },
        {
          id: 4,
          title: "React",
          img: react,
          class_name: "react",
        },
        {
          id: 5,
          title: "Node",
          img: node,
          class_name: "node",
        },
        {
          id: 6,
          title: "MongoDB",
          img: mongodb,
          class_name: "mongodb",
        },
        {
          id: 7,
          title: "Vue",
          img: vue,
          class_name: "vue",
        },
        {
          id: 8,
          title: "Anguler",
          img: angular,
          class_name: "anguler",
        },
      ],
    };
  },
};
</script>

