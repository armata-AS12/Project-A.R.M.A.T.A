<template>
  <section class="main-banner">
      <div class="content">
          <h1>ระบบเช็คชื่อสแกนหน้า ประจําวัน</h1>
          <button @click="checkIn">เช็คชื่อ</button>
          <br><button @click="ACDC">ลงทะเบียน</button>
      </div>
  </section>

    <!-- Footer Section -->
        <div class="footer-content">
            <!-- Footer Links... -->
        </div>
</template>
<script setup>
import { useRouter } from 'vue-router';
const router = useRouter();
const checkIn = () => {
    //โค้ดส่วนนี้สำหรับเชื่อมต่อไปยังหน้า เช็คชื่อ แต่ถ้าไม่ได้ login จะทำให้ไปยังหน้า Login
    router.push('/listactivities')
}
const ACDC = () => {
    //โค้ดส่วนนี้สำหรับเชื่อมต่อไปยังหน้า เช็คชื่อ แต่ถ้าไม่ได้ login จะทำให้ไปยังหน้า Login
    router.push('/liststaff')
}
</script>

<!-- นำเข้าไฟล์ CSS จาก assets/style/homepage.css -->
<style src="~/assets/style/homepage.css"></style>