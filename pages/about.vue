<template>
  <v-container fluid class="about-section">
    <!-- ヒーローセクション（背景画像付き） -->
    <v-row align="center" justify="center" class="about-hero">
      <v-col cols="12" md="10" class="text-center">
        <h1 class="about-title animate-title">会社概要</h1>
        <p class="about-subtitle animate-subtitle">
          信頼・技術・安全を第一に、日本の未来を支える企業
        </p>
      </v-col>
    </v-row>

    <!-- 代表挨拶 -->
    <v-container class="ceo-section">
      <v-row align="center">
        <v-col cols="12" md="6">
          <!-- 外部画像を利用 -->
          <v-img
            src="/ippuku.jpg"
            class="ceo-img"
          ></v-img>
        </v-col>
        <v-col cols="12" md="6">
          <h2 class="ceo-title">代表挨拶</h2>
<p class="ceo-message">
  ACE興管は2004年の創業以来、都市ガス配管工事のリーディングカンパニーとして、日本のエネルギーインフラを支えてまいりました。  
  年間1,000世帯以上の施工実績を誇り、超高層ビルの新築工事から保安業務に至るまで、確かな技術力と迅速な対応力でお客様から高い評価を頂いております。  
  <br /><br />
  施工品質の高さは業界内でもトップクラス。「配管が美しい」「対応が迅速で助かった」との声が多数寄せられています。  
  また、カンボジアをはじめとするグローバル展開にも積極的に取り組み、日本基準の技術を海外へ輸出。現地人材の育成にも力を入れています。  
  <br /><br />
  私たちの成功の鍵は、社員の成長環境と挑戦の機会です。  
  平均5年で現場を任され、職長昇進後わずか2〜3年で年収800万円超えのキャリアパスが実現可能な環境を整えています。  
  <br /><br />
  未来のエネルギー供給を見据え、最新技術の導入・品質向上・環境配慮を徹底し、業界のさらなる発展に貢献してまいります。  
  ACE興管は、国内最高水準の施工技術とグローバル展開を軸に、次なるステージへと進み続けます。  
  <br /><br />
  これからも変わらぬご支援・ご愛顧を賜りますよう、心よりお願い申し上げます。
</p>
<p class="ceo-name">代表取締役 小松 洋一</p>


        </v-col>
      </v-row>
    </v-container>

    <!-- 企業情報 -->
    <v-container class="company-info">
      <h2 class="section-title">企業情報</h2>
      <v-row>
        <v-col cols="12" md="6">
          <v-card class="info-card">
            <v-card-title>会社名</v-card-title>
            <v-card-text>有限会社エース興管</v-card-text>
          </v-card>
          <v-card class="info-card">
            <v-card-title>設立</v-card-title>
            <v-card-text>2004年12月1日</v-card-text>
          </v-card>
          <v-card class="info-card">
            <v-card-title>代表者</v-card-title>
            <v-card-text>小松 洋一</v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="6">
          <v-card class="info-card">
            <v-card-title>所在地</v-card-title>
            <v-card-text>東京都江戸川区江戸川６丁目３１－１４７</v-card-text>
          </v-card>
          <v-card class="info-card">
            <v-card-title>資本金</v-card-title>
            <v-card-text>3百万円</v-card-text>
          </v-card>
          <v-card class="info-card">
            <v-card-title>事業内容</v-card-title>
            <v-card-text>都市ガス配管工事、商業施設設備工事、メンテナンス・保守</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>


<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600&family=Noto+Sans+JP:wght@300;400;700&display=swap');

* {
  font-family: 'Poppins', 'Noto Sans JP', sans-serif;
}

/* ヒーローセクション */

.about-hero {
  background-image: url('https://images.pexels.com/photos/3184312/pexels-photo-3184312.jpeg');
  background-size: cover !important;
  background-position: center !important;
  background-repeat: no-repeat !important;
  height: 60vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  color: white;
  position: relative;
}

.about-hero::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background: rgba(0, 0, 0, 0.5);
}

.about-title {
  font-size: 3rem;
  font-weight: bold;
  text-shadow: 3px 3px 10px rgba(0, 0, 0, 0.3);
  animation: fadeIn 1.5s ease-in-out;
}

.about-subtitle {
  font-size: 1.4rem;
  opacity: 0.9;
  animation: fadeIn 2s ease-in-out;
}

/* 代表挨拶 */
.ceo-section {
  padding: 100px 20px;
  text-align: left;
}

.ceo-img {
  border-radius: 10px;
  width: 100%;
  box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
}

.ceo-title {
  font-size: 2rem;
  font-weight: bold;
}

.ceo-message {
  font-size: 1.2rem;
  margin-top: 20px;
  line-height: 1.8;
}

.ceo-name {
  font-size: 1.3rem;
  font-weight: bold;
  margin-top: 20px;
}

/* 企業情報 */
.company-info {
  background: #a9aaac;
  padding: 80px 20px;
  text-align: center;
}

.section-title {
  font-size: 2rem;
  font-weight: bold;
  margin-bottom: 40px;
}

.info-card {
  padding: 20px;
  margin-bottom: 20px;
  border-radius: 10px;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
}

.info-card .v-card-title {
  font-size: 1.3rem;
  font-weight: bold;
}

.info-card .v-card-text {
  font-size: 1.2rem;
}

/* アニメーション */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(10px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

