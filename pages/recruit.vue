<template>
  <v-container fluid class="recruit-section">
    <!-- ヒーローセクション -->
    <v-row align="center" justify="center" class="hero-content">
      <v-col cols="12" md="10" class="text-center">
        <h1 class="hero-title animate-title">採用情報</h1>
        <p class="hero-description animate-description">
          ACE興管は、あなたの成長と未来を全力でサポートします。
        </p>
      </v-col>
    </v-row>

    <!-- 会社の魅力 -->
    <v-container class="company-overview">
      <h2 class="section-title">ACE興管で働く魅力</h2>
      <v-row justify="center">
        <v-col cols="12" md="4">
          <v-card class="feature-card">
            <v-icon size="50" class="gold-icon">mdi-school</v-icon>
            <v-card-title>充実の研修制度</v-card-title>
            <v-card-text>未経験でも基礎から学べる安心の研修あり</v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="feature-card">
            <v-icon size="50" class="gold-icon">mdi-certificate</v-icon>
            <v-card-title>資格取得支援</v-card-title>
            <v-card-text>スキルアップを応援！費用負担で資格取得</v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="feature-card">
            <v-icon size="50" class="gold-icon">mdi-handshake</v-icon>
            <v-card-title>安心の職場環境</v-card-title>
            <v-card-text>仲間と支え合い、安心して働ける環境</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>

    <!-- 募集要項 -->
<v-container class="job-listing">
  <h2 class="section-title">募集職種 & 募集要項</h2>
  <v-expansion-panels class="job-panels">
    <v-expansion-panel>
      <v-expansion-panel-title>
        ガス配管工事スタッフ（正社員／借り上げマンション完備で地方出身者歓迎／資格取得・独立支援制度あり）
      </v-expansion-panel-title>
      <v-expansion-panel-text>
        <div class="job-description">

          <!-- 業務内容 -->
          <h3 class="job-subheading">仕事内容</h3>
          <p>
            新設マンション・学校・ビル等のガス配管工事（新設・回収）を担当。<br>
            チームで2〜4名体制。現場を一人で任せることはありません。<br>
            最初は簡単な作業からスタートし、先輩の指導のもと着実に成長できます。
          </p>

          <!-- 働く環境 -->
          <h3 class="job-subheading">職場の特徴</h3>
          <p>
            和気あいあいとした雰囲気で、質問しやすく人間関係も良好。<br>
            スタッフの約半数が15年以上在籍しており、定着率・安心感が抜群です。<br>
            地方出身者には借り上げマンション（寮）を完備。すぐに新生活を始められます。
          </p>

          <!-- 募集条件 -->
          <h3 class="job-subheading">募集条件・待遇</h3>
          <ul class="job-list">
            <li><strong>雇用形態：</strong> 正社員（試用期間3ヶ月・同条件）</li>
            <li><strong>給与：</strong> 月給20万円〜40万円（研修時は日給1万円）★昇給あり</li>
            <li><strong>勤務地：</strong> 東京都練馬区／江戸川区／埼玉県新座市（倉庫）など ※現場による</li>
            <li><strong>アクセス：</strong> 武蔵関駅・一之江駅・船堀駅・葛西駅 徒歩圏内</li>
            <li><strong>勤務時間：</strong> 8:00〜17:00（現場により変動あり）</li>
            <li><strong>休日・休暇：</strong> 日曜・祝日、夏季休暇、年末年始休暇</li>
            <li><strong>福利厚生：</strong> 交通費全額支給、髪型自由、直行直帰OK、<br>
              借り上げマンション完備、資格取得支援（ガス配管1〜3種）、<br>
              独立支援制度、社会保険完備、社員旅行</li>
            <li><strong>応募資格：</strong> 高卒以上、学歴・年齢不問、未経験歓迎</li>
            <li><strong>歓迎条件：</strong> 建築業界経験者、普通自動車免許（AT可）、<br>
              配管工事関連資格保持者は優遇</li>
          </ul>
        </div>
      </v-expansion-panel-text>
    </v-expansion-panel>
  </v-expansion-panels>
</v-container>

    <!-- 応募方法 -->
    <v-container class="apply-section">
      <h2 class="section-title">応募方法</h2>
      <v-row justify="center">
        <v-col cols="12" md="4">
          <v-card class="apply-card">
            <v-icon size="50" class="gold-icon">mdi-email</v-icon>
            <v-card-title>書類応募</v-card-title>
            <v-card-text>履歴書をメールで送信</v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="apply-card">
            <v-icon size="50" class="gold-icon">mdi-account-check</v-icon>
            <v-card-title>面接</v-card-title>
            <v-card-text>リラックスした雰囲気で面接</v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="apply-card">
            <v-icon size="50" class="gold-icon">mdi-briefcase-check</v-icon>
            <v-card-title>内定・入社</v-card-title>
            <v-card-text>新しい仲間として歓迎します！</v-card-text>
          </v-card>
        </v-col>
      </v-row>
      <div class="cta-buttons">
        <v-btn class="cta-btn primary-btn" to="/contact">応募する</v-btn>
      </div>
    </v-container>
  </v-container>

  <v-container fluid class="employee-voice-section">
    <!-- セクション2: 働いている人の声 -->
    <v-container class="employee-voice">
      <h2 class="section-title">働いている人の声</h2>
      <p class="employee-intro">ACE興管には25名の従業員が在籍し、地域最大のガス配管工事会社として活躍しています。<br>
      働きやすい環境、やさしい先輩、資格制度や充実した研修が、皆が集まる理由です。</p>

      <v-row justify="center">
        <v-col cols="12" md="6">
          <v-card class="employee-card">
            <v-card-title>30代・職長</v-card-title>
            <v-card-text>
              「未経験から始めましたが、平均5年で現場を任せてもらえました。
              職長になってからわずか2〜3年で年収800万円を超えることができました！」
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="6">
          <v-card class="employee-card">
            <v-card-title>20代・新人</v-card-title>
            <v-card-text>
              「先輩たちがとても優しく、資格取得もサポートしてくれるので安心して仕事を覚えることができました！」
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>

      <!-- 追加の社員の声 -->
      <v-row justify="center">
        <v-col cols="12" md="6">
          <v-card class="employee-card">
            <v-card-title>40代・ベテラン</v-card-title>
            <v-card-text>
              「ACE興管には長く働ける環境が整っています。
              仕事の安定感があり、家族を支えながらキャリアアップできる点が魅力です。」
            </v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="6">
          <v-card class="employee-card">
            <v-card-title>50代・管理職</v-card-title>
            <v-card-text>
              「若手がどんどん育ち、会社全体の成長を実感しています。
              経験を積むことで高収入も可能なので、やる気のある人には最高の職場です！」
            </v-card-text>
          </v-card>
        </v-col>
      </v-row>

      <!-- 成長環境・キャリアパス -->
      <h2 class="section-title">ACE興管の成長環境 & キャリアパス</h2>
      <p class="growth-intro">社員一人ひとりが成長できる環境を整備し、スキルアップをサポートしています。<br>
      努力次第で早期昇進も可能で、収入アップも夢ではありません。</p>

      <v-row justify="center">
        <v-col cols="12" md="4">
          <v-card class="feature-card">
            <v-icon size="50" class="gold-icon">mdi-school</v-icon>
            <v-card-title>実践的な研修</v-card-title>
            <v-card-text>現場に即した実践的な研修でスキルアップ</v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="feature-card">
            <v-icon size="50" class="gold-icon">mdi-certificate</v-icon>
            <v-card-title>キャリアアップ支援</v-card-title>
            <v-card-text>資格取得だけでなく職長への昇進もサポート</v-card-text>
          </v-card>
        </v-col>
        <v-col cols="12" md="4">
          <v-card class="feature-card">
            <v-icon size="50" class="gold-icon">mdi-cash-multiple</v-icon>
            <v-card-title>収入アップのチャンス</v-card-title>
            <v-card-text>経験を積めば短期間で年収800万円超えも可能</v-card-text>
          </v-card>
        </v-col>
      </v-row>
    </v-container>
  </v-container>
</template>


<style scoped>
/* 🎨 高級感のある背景 */
.recruit-section {
  background: linear-gradient(to right, #a2b8e4, #2d3c63);
  color: white;
  padding-top: 120px;
  padding-bottom: 80px;
}

/* 🎨 ヘッダー */
.hero-title {
  font-size: 3.8rem;
  font-weight: 700;
  text-shadow: 3px 3px 10px rgba(255, 215, 0, 0.5);
  animation: fadeIn 1.5s ease-in-out;
}

.hero-description {
  font-size: 1.3rem;
  max-width: 800px;
  margin: 0 auto 40px;
  animation: fadeIn 1.4s ease-in-out;
  text-shadow: 1px 1px 6px rgba(0, 0, 0, 0.5);
}

/* 🎨 ゴールドのアイコン */
.gold-icon {
  color: #d4af37 !important;
}

/* 🎨 募集要項 */
.job-listing {
  background: #ffffff;
  color: #0c1b3a;
  padding: 80px 40px;
  text-align: left;
  border-radius: 12px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.15);
  line-height: 1.8;
  font-size: 1rem;
}

.section-title {
  font-size: 2.4rem;
  font-weight: 800;
  color: #0c1b3a;
  margin-bottom: 30px;
  border-bottom: 4px solid #d4af37;
  display: inline-block;
  padding-bottom: 12px;
}

.job-text {
  font-size: 1.2rem;
  font-weight: 600;
  margin-bottom: 20px;
}

.job-list {
  padding-left: 0;
}

.job-list li {
  font-size: 1rem;
  margin-bottom: 14px;
  padding-left: 1.5rem;
  position: relative;
  list-style: none;
}

.job-list li::before {
  content: "\2022";
  color: #d4af37;
  font-weight: bold;
  display: inline-block;
  width: 1rem;
  margin-left: -1.5rem;
  position: absolute;
  top: 0.2rem;
}

.job-subheading {
  font-size: 1.3rem;
  font-weight: 700;
  color: #0c1b3a;
  margin-top: 30px;
  margin-bottom: 10px;
  border-left: 5px solid #d4af37;
  padding-left: 12px;
}

.job-description p {
  line-height: 1.8;
  margin-bottom: 20px;
}

.job-list li {
  margin-bottom: 10px;
  line-height: 1.6;
}


/* 🎨 応募方法 */
.apply-section {
  background: #f5f5f5;
  padding: 100px 40px;
  text-align: center;
  color: #0c1b3a;
}

/* 🎨 CTAボタン（応募するボタン） */
.cta-buttons {
  margin-top: 50px;
  display: flex;
  justify-content: center;
}

.primary-btn {
  background: linear-gradient(135deg, #fcd964, #d4af37);
  color: #1c1c1c;
  border: none;
  font-size: 1.4rem;
  padding: 14px 38px;
  border-radius: 40px;
  font-weight: 800;
  letter-spacing: 1px;
  display: flex;
  align-items: center;
  justify-content: center;
  min-width: 200px;
  transition: all 0.3s ease-in-out;
  box-shadow: 0 6px 20px rgba(212, 175, 55, 0.4);
}

.primary-btn:hover {
  background: linear-gradient(135deg, #d4af37, #a8862a);
  transform: scale(1.05);
  box-shadow: 0 10px 30px rgba(212, 175, 55, 0.6);
}

/* 🎨 アニメーション */
@keyframes fadeIn {
  from { opacity: 0; transform: translateY(10px); }
  to { opacity: 1; transform: translateY(0); }
}
</style>

<style scoped>
.employee-voice-section {
  background: linear-gradient(to right, #f4f4f4, #d9e2ec);
  padding: 100px 20px;
  text-align: center;
}

.section-title {
  font-size: 2.8rem;
  font-weight: bold;
  color: #0c1b3a;
  margin-bottom: 30px;
  border-bottom: 4px solid #e0c07c;
  display: inline-block;
  padding-bottom: 10px;
}

.employee-intro, .growth-intro {
  font-size: 1.4rem;
  font-weight: 400;
  max-width: 850px;
  margin: 0 auto 50px;
  color: #333;
  line-height: 1.6;
}

.employee-card, .feature-card {
  padding: 40px;
  border-radius: 12px;
  background: white;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.2);
  transition: transform 0.3s ease-in-out;
  text-align: left;
}

.employee-card:hover, .feature-card:hover {
  transform: scale(1.08);
}

.employee-card v-card-title, .feature-card v-card-title {
  font-size: 1.5rem;
  font-weight: bold;
  color: #0c1b3a;
}

.employee-card v-card-text, .feature-card v-card-text {
  font-size: 1.2rem;
  color: #555;
}

.gold-icon {
  color: #d4af37 !important;
}
</style>

