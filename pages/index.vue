<template>
  <v-container fluid class="home-section">
    <!-- ヒーローセクション -->
    <v-row align="center" justify="center" class="hero-content">
      <v-col cols="12" md="10" class="text-center home-content">
        <h2 class="hero-subtitle animate-subtitle">技術 × 品質 × 信頼</h2>
        <h1 class="hero-title animate-title">ACE興管</h1>
        <p class="hero-description animate-description">
          卓越した技術力と誠実な施工で、<br />
          ACE興管はガスインフラの未来を築くプロフェッショナル集団です。<br />
          私たちは「暮らしの安全と快適」を支える誇りを胸に、常に最前線で挑み続けています。
        </p>
        <div class="cta-buttons">
          <router-link to="/about">
            <v-btn class="cta-btn primary-btn">会社概要</v-btn>
          </router-link>
        </div>
      </v-col>
    </v-row>

    <!-- 事業内容 -->
    <v-container class="service-overview">
      <h2 class="section-title">事業内容</h2>
      <h3 class="section-description">
        ACE興管は、新築マンションを中心に、学校・店舗などの新設工事、<br />
        老朽化したガス設備の保守・改修など、幅広いガス工事を通じて社会を支えています。<br />
        豊富な実績と現場対応力を活かし、すべてのお客様に安心をお届けします。
      </h3>
      <v-row justify="center">
        <v-col cols="12" md="4">
          <v-card class="service-card">
            <v-icon size="60" class="gold-icon">mdi-office-building</v-icon>
            <v-card-title>新築マンション施工</v-card-title>
            <v-card-text>
              当社の主力分野。新築集合住宅のインフラ整備において、<br />
              初期設計から施工まで一貫して対応します。
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="service-card">
            <v-icon size="60" class="gold-icon">mdi-storefront-outline</v-icon>
            <v-card-title>学校・店舗施工</v-card-title>
            <v-card-text>
              教育施設・商業施設など、多様な現場に最適な配管工事を提供。<br />
              現場に合わせた柔軟な施工体制が強みです。
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="service-card">
            <v-icon size="60" class="gold-icon">mdi-shield-check</v-icon>
            <v-card-title>保安・改修工事</v-card-title>
            <v-card-text>
              老朽化した設備の点検・改修を通じて、<br />
              事故防止と長期的な安心を実現します。
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
      <v-row align="center" justify="center">
        <v-col cols="12" md="10" class="text-center">
          <div class="cta-buttons">
            <router-link to="/services">
              <v-btn class="cta-btn primary-btn">もっと見る</v-btn>
            </router-link>
          </div>
        </v-col>
      </v-row>
    </v-container>


    <!-- 働く環境 -->
    <v-container class="work-environment">
      <h2 class="section-title">ACE興管の働く環境</h2>
      <h3 class="section-description">
        従業員が楽しく、そして誇りを持って働ける職場づくりをしています。<br />
        未経験でも安心の研修制度と充実の福利厚生を完備。<br />
        「人が育つ会社」で、一緒に未来を創りませんか？
      </h3>
      <v-row justify="center">
        <v-col cols="12" md="4">
          <v-card class="work-card">
            <v-icon size="60" class="gold-icon">mdi-account-group</v-icon>
            <v-card-title>チームワーク</v-card-title>
            <v-card-text>
              社員同士のサポート体制が充実！<br />
              困ったときはみんなで助け合う文化。
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="work-card">
            <v-icon size="60" class="gold-icon">mdi-lightbulb-on</v-icon>
            <v-card-title>キャリア成長</v-card-title>
            <v-card-text>
              研修制度が充実し、未経験からでもプロへ！<br />
              資格取得サポートあり。
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="work-card">
            <v-icon size="60" class="gold-icon">mdi-emoticon-happy</v-icon>
            <v-card-title>安心の福利厚生</v-card-title>
            <v-card-text>
              各種手当・社会保険完備！<br />
              長く働ける環境を提供。
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>
      <v-row align="center" justify="center">
        <v-col cols="12" md="10" class="text-center">
          <div class="cta-buttons">
            <router-link to="/recruit">
              <v-btn class="cta-btn primary-btn">もっと見る</v-btn>
            </router-link>
          </div>
        </v-col>
      </v-row>
    </v-container>

    <!-- CTAセクション -->
    <v-container class="cta-section">
      <h2 class="section-title">一緒に未来を創りましょう</h2>
      <h3 class="cta-text">
        技術 × チームワーク × 成長<br />
        最高の環境で、一緒に成長しませんか？<br />
        求職者の方も、クライアントの方も、お気軽にお問い合わせください。
      </h3>
      <div class="cta-buttons">
        <router-link to="/contact">
          <v-btn class="cta-btn secondary-btn">お問い合わせ</v-btn>
        </router-link>
      </div>
    </v-container>
  </v-container>
</template>


<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Noto+Serif+JP:wght@500;700&display=swap');

* {
  font-family: 'Playfair Display', 'Noto Serif JP', serif;
  box-sizing: border-box;
}

/* 🌇 高級感のある背景と適度な暗さの調整 */
.home-section {
  background-image: url('/images/haikann10.jpg');
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
  position: relative;
  color: white;
  padding: 140px 0;
}

.home-section::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.18);
  z-index: 0;
}

.home-content {
  position: relative;
  z-index: 2;
  text-align: center;
  max-width: 1200px;
  margin: 0 auto;
}

/* 🏷️ タイトルデザイン 3D強化 + ゴールド光彩 */
.hero-title {
  font-size: 5rem;
  font-weight: 800;
  color: #fff;
  text-shadow:
    1px 1px 0 #d4af37,
    2px 2px 3px rgba(0, 0, 0, 0.9),
    4px 4px 10px rgba(255, 215, 0, 0.6);
  animation: fadeIn 1.5s ease-in-out;
  letter-spacing: 3px;
  margin-bottom: 24px;
}

.hero-description {
  font-size: 1.7rem;
  max-width: 960px;
  margin: 0 auto 60px;
  color: #fdfdfd;
  text-shadow: 2px 2px 6px rgba(0, 0, 0, 0.85);
  line-height: 1.8;
}

.section-title {
  font-size: 3.5rem;
  font-weight: 800;
  color: #fff;
  border-bottom: 5px solid #ffda73;
  display: inline-block;
  padding-bottom: 14px;
  text-shadow:
    1px 1px 0 #d4af37,
    2px 2px 3px rgba(0, 0, 0, 0.7);
  letter-spacing: 2px;
  margin-bottom: 40px;
}

/* 📦 カードデザインと明るさ調整 */
.service-card, .work-card {
  background: rgba(255, 255, 255, 0.35);
  border: 1px solid rgba(255, 255, 255, 0.5);
  backdrop-filter: blur(12px);
  box-shadow: 0 12px 35px rgba(0, 0, 0, 0.4);
  padding: 42px;
  border-radius: 18px;
  text-align: center;
  color: #fff;
  transition: all 0.3s ease-in-out;
}

.service-card:hover, .work-card:hover {
  background: rgba(255, 255, 255, 0.5);
  transform: scale(1.06);
  box-shadow: 0 18px 50px rgba(255, 215, 0, 0.7);
}

.service-card .v-card-title, .work-card .v-card-title {
  font-size: 1.9rem;
  font-weight: bold;
  color: #e0c07c;
  margin-bottom: 12px;
  text-shadow: 2px 2px 6px rgba(0, 0, 0, 0.8);
}

.service-card .v-card-text, .work-card .v-card-text {
  font-size: 1.3rem;
  line-height: 1.8;
  color: #ffffff;
  text-shadow: 1px 1px 3px rgba(0, 0, 0, 0.7);
}

/* 🟡 ゴールドアイコンに変更 */
.gold-icon {
  color: #e0c07c !important;
  font-size: 3rem;
  margin-bottom: 20px;
}

/* ✨ ボタンリッチな装飾とアニメーション */
.cta-btn {
  font-size: 1.5rem;
  padding: 14px 36px;
  border-radius: 50px;
  font-weight: 800;
  text-transform: uppercase;
  transition: all 0.3s ease-in-out;
  display: inline-flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.45);
  cursor: pointer;
  letter-spacing: 1.2px;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.5);
  position: relative;
  overflow: hidden;
}

.primary-btn {
  background: linear-gradient(145deg, #ffd700, #e0c04e);
  color: #1b1b1b;
  border: 2px solid #fff3c4;
}

.primary-btn:hover {
  background: linear-gradient(145deg, #e0c04e, #caa93a);
  box-shadow: 0 10px 32px rgba(255, 215, 0, 0.6);
  transform: translateY(-2px);
}

.secondary-btn {
  background: linear-gradient(to right, #fff0b3, #ffcc00);
  color: #1a1a1a;
  border: 2px solid #e6c300;
  animation: pulseGlow 2s infinite;
}

.secondary-btn:hover {
  background: linear-gradient(to right, #ffe066, #ffd700);
  box-shadow: 0 8px 24px rgba(255, 223, 0, 0.6);
  transform: translateY(-2px);
}

.cta-btn:active {
  transform: scale(0.96);
}

/* 🔁 CTAのアニメーション */
@keyframes pulseGlow {
  0% {
    box-shadow: 0 0 10px rgba(255, 215, 0, 0.4);
  }
  50% {
    box-shadow: 0 0 20px rgba(255, 215, 0, 0.8);
  }
  100% {
    box-shadow: 0 0 10px rgba(255, 215, 0, 0.4);
  }
}

/* 📱 モバイル対応 */
@media (max-width: 768px) {
  .hero-title {
    font-size: 3.2rem;
  }

  .hero-description {
    font-size: 1.3rem;
  }

  .section-title {
    font-size: 2.6rem;
  }

  .cta-buttons {
    flex-direction: column;
  }
}

@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}
</style>
