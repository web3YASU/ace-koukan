<script setup lang="ts">
import { ref } from 'vue';

const name = ref('');
const email = ref('');
const message = ref('');
const successMessage = ref('');

const submitForm = () => {
  if (name.value && email.value && message.value) {
    successMessage.value = 'お問い合わせを受け付けました。近日中にご連絡いたします。';
    name.value = '';
    email.value = '';
    message.value = '';
  }
};
</script>

<template>
  <v-container fluid class="contact-section">
    <!-- タイトル -->
    <v-row align="center" justify="center">
      <v-col cols="12" md="8" class="text-center">
        <h1 class="contact-title">お問い合わせ</h1>
        <p class="contact-subtitle">
          サービスに関するご相談・お問い合わせは、以下のフォームよりお気軽にご連絡ください。
        </p>
      </v-col>
    </v-row>

    <!-- お問い合わせフォーム -->
    <v-container class="form-container">
      <v-row justify="center">
        <v-col cols="12" md="6">
          <v-card class="form-card">
            <v-card-title>お問い合わせフォーム</v-card-title>
            <v-card-text>
              <v-text-field v-model="name" label="お名前" required outlined></v-text-field>
              <v-text-field v-model="email" label="メールアドレス" type="email" required outlined></v-text-field>
              <v-textarea v-model="message" label="お問い合わせ内容" required outlined></v-textarea>
              <v-btn color="primary" block large @click="submitForm">送信</v-btn>
              <p v-if="successMessage" class="success-message">{{ successMessage }}</p>
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <!-- 会社情報と所在地 -->
    <v-container fluid class="info-section">
      <v-row justify="center">
        <v-col cols="12" md="5">
          <h2 class="section-title">会社情報</h2>
          <p><strong>会社名:</strong> 有限会社ACE興管</p>
          <p><strong>所在地:</strong> 東京都江戸川区江戸川６丁目３１－１４７</p>
          <p><strong>電話番号:</strong> 03-6808-2778</p>
          <p><strong>メール:</strong> info@ace-koukan.co.jp</p>
          <p><strong>営業時間:</strong> 平日 9:00 - 18:00</p>
        </v-col>
        <v-col cols="12" md="5">
          <!-- Google Map 埋め込み -->
          <v-img src="https://source.unsplash.com/600x400/?map,city" class="map-image"></v-img>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>

<style scoped>
/* Google Fonts */
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Noto+Sans+JP:wght@300;400;700&display=swap');

* {
  font-family: 'Poppins', 'Noto Sans JP', sans-serif;
}

/* メイン背景 */
.contact-section {
  background: linear-gradient(to right, #1e1e1e, #2c3e50);
  color: white;
  padding: 60px 20px;
}

/* タイトル */
.contact-title {
  font-size: 3rem;
  font-weight: 700;
  text-transform: uppercase;
  letter-spacing: 1.5px;
  text-align: center;
}

.contact-subtitle {
  font-size: 1.3rem;
  font-weight: 300;
  opacity: 0.9;
  max-width: 800px;
  margin: 0 auto;
  text-align: center;
}

/* フォームコンテナ */
.form-container {
  padding: 50px 0;
}

/* フォームカード */
.form-card {
  padding: 30px;
  border-radius: 12px;
  background: white;
  color: #333;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

.success-message {
  color: #27ae60;
  font-size: 1.2rem;
  margin-top: 10px;
}

/* 会社情報セクション */
.info-section {
  background: #f8f9fa;
  padding: 50px 20px;
  color: #222;
}

/* 地図 */
.map-image {
  border-radius: 12px;
  width: 100%;
  object-fit: cover;
}
</style>
