<template>
  <div class="cv-container">
    <div class="left-column">
      <div class="profile-box">
        <div class="profile-pic" style="background-image: url('assets/img/profile.jpeg');"></div>
        <h1>Yoga Muhammad Fauzi</h1>
        <p class="university">Universitas Brawijaya</p>
      </div>
    </div>

    <div class="right-column">
      <section class="career-goal">
        <h2>Tentang Saya</h2>
        <p class="goal-description">Saya adalah mahasiswa Universitas Brawijaya dari Jurusan Teknologi Informasi Fakultas Vokasi. Saya ingin menjadi seorang programmer.</p>
        <div class="dotted-line"></div>
      </section>

      <section class="personal-info">
        <ul>
          <li><strong>Tanggal Lahir:</strong> <span class="info">14 Maret 2004</span></li>
          <li><strong>Alamat:</strong> <span class="info">Jl. Bendi Gang Arjuna Nomor A6, Kota Probolinggo, Jawa Timur, Indonesia</span></li>
          <li><strong>Nomor Telepon:</strong> <span class="info">+62 899 9316 537</span></li>
          <li><strong>Email:</strong> <span class="info">yogamfauzi@email.com</span></li>
        </ul>
      </section>
    </div>
  </div>
</template>

<style scoped>
.cv-container {
  position: relative;
  display: flex;
  height: 100vh;
  font-family: 'Arial', sans-serif;
  padding: 20px;
  color: #ffffff;
  z-index: 1;
}

.cv-container::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-image: url('assets/img/background.jpg');
  background-size: cover;
  background-position: center;
  opacity: 0.7;
  z-index: -1;
}

.cv-container::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.5);
  z-index: -1;
}

.left-column {
  width: 35%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.profile-box {
  text-align: center;
  border: 2px solid #00bfff;
  padding: 40px;
  border-radius: 10px;
}

.profile-pic {
  width: 150px;
  height: 150px;
  border-radius: 50%;
  background-color: #f0f0f0;
  margin: 0 auto 20px;
  background-size: cover;
  background-position: center;
}

h1 {
  font-size: 1.8em;
  color: #ffffff;
}

.university {
  color: #ffffff;
}

.right-column {
  width: 65%;
  padding-left: 40px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.career-goal h2 {
  font-size: 1.6em;
  margin-bottom: 10px;
  color: #00bfff;
}

.career-goal .goal-description {
  font-size: 1.2em;
  margin-bottom: 20px;
  color: #ffffff;
}

.dotted-line {
  width: 100%;
  border-top: 2px dotted #00bfff;
  margin: 20px 0;
}

.personal-info ul {
  list-style-type: none;
  padding: 0;
}

.personal-info li {
  font-size: 1.2em;
  margin-bottom: 10px;
  color: #ffffff;
}

.personal-info strong {
  color: #00bfff;
}

.info {
  color: #ffffff;
}
</style>
