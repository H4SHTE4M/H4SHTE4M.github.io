---
layout: article
titles:
  # @start locale config
  en      : &EN       About
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
  zh-Hans : &ZH_HANS  关于
  zh      : *ZH_HANS
  zh-CN   : *ZH_HANS
  zh-SG   : *ZH_HANS
  zh-Hant : &ZH_HANT  關於
  zh-TW   : *ZH_HANT
  zh-HK   : *ZH_HANT
  ko      : &KO       소개
  ko-KR   : *KO
  fr      : &FR       À propos
  fr-BE   : *FR
  fr-CA   : *FR
  fr-CH   : *FR
  fr-FR   : *FR
  fr-LU   : *FR
  # @end locale config
key: page-about
---

<style>
.container {
  display: grid;
  grid-template-columns: 2fr 1fr;
  grid-template-rows: auto;
  gap: 20px;
  padding: 20px;
  font-family: Arial, sans-serif;
}

.container2 {
  display: grid;
  grid-template-columns: 1fr 2fr;
  grid-template-rows: auto;
  gap: 20px;
  padding: 20px;
  font-family: Arial, sans-serif;
}

.logo {
  grid-column: 1 / 3;
  text-align: center;
}


.logo img {
  border-radius: 50%;
  background-color: #f0f0f0;
  padding: 10px;
}

.about, .achievements, .skills, .history, .join-us {
  background-color: #f4f4f4;
  padding: 20px;
  border-radius: 10px;
}

h1, h2 {
  color: #333;
}

p, ul {
  color: #666;
  line-height: 1.6;
}

ul {
  list-style-type: disc;
  margin-left: 20px;
}

.skills-chart {
  display: flex;
  justify-content: center;
  align-items: center;
}

.timeline {
  display: flex;
  justify-content: space-between;
  align-items: center;
  position: relative;
  padding: 20px 0;
  height: 200px;
}

.timeline .event {
  text-align: center;
  position: relative;
  width: 20%;
}

.timeline .event span {
  display: block;
}

.timeline .event span:first-child {
  margin-bottom: 40px; /* 增加时间与事件之间的间距 */
}

.timeline:before {
  content: '';
  position: absolute;
  top: 50%;
  left: 0;
  width: 100%;
  height: 2px;
  background-color: #ccc;
}

.timeline:after {
  content: '';
  position: absolute;
  top: 50%;
  right: -5px;
  transform: translateY(-50%);
  width: 0;
  height: 0;
  border-top: 10px solid transparent;
  border-bottom: 10px solid transparent;
  border-left: 10px solid #ccc;
}

.timeline .event:before {
  content: '';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 10px;
  height: 10px;
  background-color: #666;
  border-radius: 50%;
}

.join-us {
  grid-column: 1 / 3;
  text-align: center;
}

.join-button {
  display: inline-block;
  margin-top: 20px;
  padding: 10px 20px;
  background-color: #007bff;
  color: #fff;
  text-decoration: none;
  border-radius: 5px;
}

.join-button:hover {
  background-color: #0056b3;
}
</style>

<div class="logo">
    <img src="https://s2.loli.net/2024/06/07/7vdFaYn3gSL2Csf.png" alt="HASHTEAM Logo" width="100" height="100">
    <h1><strong>HASHTEAM</strong></h1>
</div>

<div class="container">
  <div class="about">
    <h2>关于我们</h2>
    <p>我们是山东大学的一个CTF战队，致力于网络安全知识的学习与竞赛。</p>
  </div>

  <div class="skills">
    <h2>技能</h2>
    <svg viewBox="0 0 120 80" xmlns="http://www.w3.org/2000/svg">
      <!-- 柱状图 -->
      <rect x="30" y="10" width="80" height="9" fill="#007bff" />
      <rect x="30" y="22" width="75" height="9" fill="#28a745" />
      <rect x="30" y="34" width="60" height="9" fill="#dc3545" />
      <rect x="30" y="46" width="65" height="9" fill="#ffc107" />
      <rect x="30" y="58" width="55" height="9" fill="#17a2b8" />
      <!-- 标签 -->
      <text x="20" y="17" text-anchor="end" font-size="6">Crypto</text>
      <text x="20" y="29" text-anchor="end" font-size="6">Pwn</text>
      <text x="20" y="41" text-anchor="end" font-size="6">Web</text>
      <text x="20" y="53" text-anchor="end" font-size="6">Reverse</text>
      <text x="20" y="65" text-anchor="end" font-size="6">Misc</text>
    </svg>
  </div>
</div>

<div class="container2">
  <div class="achievements">
    <h2>成就</h2>
    <ul>
      <li>2020年XXCTF比赛冠军</li>
      <li>2021年YYCTF比赛亚军</li>
      <li>2022年ZZCTF比赛季军</li>
      <li>2020年XXCTF比赛冠军</li>
      <li>2021年YYCTF比赛亚军</li>
      <li>2022年ZZCTF比赛季军</li>
      <li>2020年XXCTF比赛冠军</li>
      <li>2021年YYCTF比赛亚军</li>
      <li>······</li>
    </ul>
  </div>

  <div class="history">
    <h2>发展历程</h2>
    <div class="timeline">
      <div class="event">
        <span>2015年</span>
        <span>HASHTEAM成立</span>
      </div>
      <div class="event">
        <span>2018年</span>
        <span>获得第一次比赛胜利</span>
      </div>
      <div class="event">
        <span>2020年</span>
        <span>赢得全国CTF比赛冠军</span>
      </div>
      <div class="event">
        <span>2022年</span>
        <span>战队成员突破50人</span>
      </div>
    </div>
  </div>

  <div class="join-us">
    <h2>加入我们</h2>
    <p>如果你是山东大学的学生，欢迎加入我们！</p>
    <a href="mailto:contact@hasteam.com" class="join-button">联系我们</a>
  </div>
</div>
