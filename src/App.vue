<script setup>
//import "@/assets/css/pico.min.css";
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <main class="container">
    <div class="header">
      <h2>ระบบลงทะเบียนเรียนออนไลน์</h2>
      <h4>มหาวิทยาลัยแม่โจ้</h4>
    </div>
    <header class="header-margin">
      <nav>
        <RouterLink to="/">หน้าแรก</RouterLink>
        <RouterLink to="/courses">รายวิชาที่เปิด</RouterLink>
        <RouterLink to="/enrollments">ลงทะเบียนเรียนด้วยตนเอง</RouterLink>
        <RouterLink to="/mycourse">วิชาที่ลงทะเบียน</RouterLink>
      </nav>
    </header>

    <RouterView />
  </main>
</template>

<style scoped>
.header-margin {
  padding-top: 0.8em;
  padding-bottom: 0.8em;
}

nav > a {
  padding-left: 0.5em;
  padding-right: 0.5em;
}

nav > a:hover {
  background: darkolivegreen;
  color: white;
}

.header {
  background: lightgoldenrodyellow;
  text-align: center;
  padding-top: 2em;
  padding-bottom: 2em;
}
</style>
