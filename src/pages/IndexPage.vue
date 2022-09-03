<template>
  <div class="bg-cyan-1">
    <div class="row">
      <Title/>
      <Photo/>
    </div>
    <hr>
    <AcademicFormation/>
    <hr>
    <Experience/>
    <hr>
    <div class="row">
      <Courses/>
      <Skills/>
    </div>
    <hr>
  </div>
</template>

<script>
import { defineComponent } from 'vue'
import Photo from 'components/Photo.vue'
import Title from 'components/Title.vue'
import AcademicFormation from 'components/AcademicFormation.vue'
import Experience from 'components/Experience.vue'
import Courses from 'components/Courses.vue'
import Skills from 'components/Skills.vue'

export default defineComponent({
  name: 'IndexPage',
  components: {
    Photo,
    Title,
    AcademicFormation,
    Experience,
    Courses,
    Skills
  }
})
</script>
<style scoped>
  hr{
    height: 5px;
    background-color: black;
  }
  div{
    margin-left: 10px;
  }
</style>
