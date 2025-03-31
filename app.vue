<script setup lang="ts">
import { useRouter } from 'vue-router';
import { onMounted, watch } from 'vue';

const router = useRouter();

// **ルートが変更されたらスクロール位置をリセット**
watch(() => router.currentRoute.value, () => {
  window.scrollTo(0, 0);
});

onMounted(() => {
  window.scrollTo(0, 0); // 初回ロード時にもリセット
});
import { ref } from "vue";

// メニューの開閉状態
const drawer = ref(false);
</script>

<template>
  <v-app>
    <!-- ヘッダー -->
    <v-app-bar app color="transparent" elevate-on-scroll class="glass-effect">
      <v-container class="d-flex align-center">
        <!-- ロゴ -->
        <v-img src="https://via.placeholder.com/150x50?text=ACE興管" alt="ロゴ" class="logo" />
        <v-spacer></v-spacer>

        <!-- ハンバーガーメニュー（右上） -->
        <v-btn icon @click="drawer = !drawer">
          <v-icon size="32" color="gold">mdi-menu</v-icon>
        </v-btn>
      </v-container>
    </v-app-bar>

    <!-- 右側の高級感のあるメニュー -->
    <v-navigation-drawer
      v-model="drawer"
      temporary
      location="right"
      class="menu-style"
    >
      <v-list>
        <v-list-item to="/" @click="drawer = false">
          <v-list-item-title class="menu-text">🏠 ホーム</v-list-item-title>
        </v-list-item>
        <v-list-item to="/about" @click="drawer = false">
          <v-list-item-title class="menu-text">📖 会社概要</v-list-item-title>
        </v-list-item>
        <v-list-item to="/services" @click="drawer = false">
          <v-list-item-title class="menu-text">
            <v-icon class="menu-icon">mdi-office-building</v-icon> 事業内容</v-list-item-title>
        </v-list-item>
        <v-list-item to="/recruit" @click="drawer = false">
          <v-list-item-title class="menu-text">💼 採用情報</v-list-item-title>
        </v-list-item>
        <v-list-item to="/contact" @click="drawer = false">
          <v-list-item-title class="menu-text">📩 お問い合わせ</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>

    <!-- 各ページの表示 -->
    <v-main>
      <router-view />
    </v-main>

    <!-- 和モダンフッター -->
    <v-footer class="footer-style">
      <v-container class="footer-container">
        <div class="footer-content">
          <p class="footer-text">© 2025 ACE興管 | 全ての権利を保有</p>
          <v-btn class="contact-btn" to="/contact">
            <span class="contact-btn-text">お問い合わせ</span>
          </v-btn>
        </div>
      </v-container>
    </v-footer>
  </v-app>
</template>

<style scoped>
/* 🎨 フォント: おしゃれでモダンな和ゴシック */
@import url('https://fonts.googleapis.com/css2?family=Zen+Kaku+Gothic+New:wght@300;400;700&family=IBM+Plex+Sans+JP:wght@300;400;700&display=swap');

* {
  font-family: 'Zen Kaku Gothic New', 'IBM Plex Sans JP', '游ゴシック', 'Hiragino Kaku Gothic ProN', sans-serif;
}

/* 🎨 和紙風の高級感のあるヘッダー */
.glass-effect {
  backdrop-filter: blur(8px);
  background: rgba(255, 255, 255, 0.1);
  box-shadow: 0px 4px 12px rgba(0, 0, 0, 0.08);
}

/* 🎨 ロゴ */
.logo {
  height: 50px;
}

/* 🎨 メニュー（ハンバーガーメニュー） */
.menu-style {
  background-color: #1c1c1c; /* 深みのある黒 */
  border-left: 3px solid #b89c67; /* 和モダンなゴールド */
}

/* 🎨 メニューの文字 */
.menu-text {
  font-size: 1.2rem;
  font-weight: 700;
  color: #f5f5f5;
  letter-spacing: 0.03em;
  transition: color 0.2s ease;
  padding: 12px 0;
}

.menu-text:hover {
  color: #b89c67;
}

/* 🎨 フッター（和モダン） */
.footer-style {
  background: #1c1c1c;
  color: white;
  text-align: center;
  padding: 20px 0;
  border-top: 3px solid #b89c67;
}

/* 🎨 フッター内のコンテンツを中央揃え */
.footer-container {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
}

/* 🎨 フッター内のテキストとボタンを縦並び */
.footer-content {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 10px;
  width: 100%;
}

/* 🎨 フッターテキスト */
.footer-text {
  font-size: 1rem;
  margin: 0;
}

/* 🎨 お問い合わせボタン */
.contact-btn {
  background-color: transparent;
  border: 2px solid #b89c67;
  color: #b89c67;
  font-weight: bold;
  letter-spacing: 0.05em;
  padding: 12px 24px;
  font-size: 1.1rem;
  transition: background-color 0.2s ease, color 0.2s ease;
  display: flex;
  align-items: center;
  justify-content: center;
  height: 50px;
  min-width: 180px;
}

/* 🎨 ボタン内のテキストを中央揃え */
.contact-btn-text {
  display: flex;
  align-items: center;
  justify-content: center;
  line-height: 1;
}

/* 🎨 ホバー時のボタン */
.contact-btn:hover {
  background-color: #b89c67;
  color: white;
}
</style>
