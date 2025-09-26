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
        .container, .container2, .container3 {
          display: grid;
          grid-template-rows: auto;
          gap: 20px;
          padding: 10px;
          font-family: Arial, sans-serif;
        }

        .container {
          grid-template-columns: 2fr 1fr;
        }

        .container2 {
          grid-template-columns: 1fr 2fr;
        }

        .container3 {
          grid-template-columns: 1fr 1fr;
        }

        @media (max-width: 1000px) {
          .container, .container2, .container3 {
            grid-template-columns: 1fr;
          }
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

        .about, .skills, .history, .join-us {
          background-color: #f4f4f4;
          padding: 20px;
          border-radius: 10px;
        }

        .achievements{
          background-color: #f4f4f4;
          padding: 20px;
          border-radius: 10px;
          font-size: 20px;
        }

        .skills svg {
          text-align: center;
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

        /* 修改后的时间线样式 - 桌面端垂直排列 */
        .timeline {
          display: flex;
          flex-direction: column;
          position: relative;
          padding: 20px 0;
          margin-left: 20px;
        }

        .timeline:before {
          content: '';
          position: absolute;
          top: 0;
          left: 0;
          width: 4px;
          height: 100%;
          background-color: #ccc;
          border-radius: 3px;
        }

        .timeline .event {
          position: relative;
          margin-bottom: 40px;
          padding-left: 30px;
        }

        .timeline .event:last-child {
          margin-bottom: 0;
        }

        .timeline .event:before {
          content: '';
          position: absolute;
          top: 5px;
          left: -8px;
          width: 20px;
          height: 20px;
          background-color: #666;
          border-radius: 50%;
          border: 4px solid #f4f4f4;
          z-index: 1;
        }

        .timeline .event span {
          display: block;
        }

        .timeline .event span:first-child {
          font-weight: bold;
          margin-bottom: 5px;
          color: #333;
        }

        /* 移动端样式 */
        @media (max-width: 600px) {
          .timeline {
            margin-left: 10px;
          }
          
          .timeline .event {
            padding-left: 25px;
          }
          
          .timeline .event:before {
            left: -6px;
            width: 16px;
            height: 16px;
          }
        }

        .join-us {
          grid-column: 1 / 3;
          text-align: center;
        }

        .join-button {
          display: inline-block;
          margin-top: 20px;
          padding: 10px 20px;
          background: linear-gradient(120deg, #a1c4fd 0%, #c2e9fb 100%);
          color: #ffffff;
          text-decoration: none;
          border-radius: 5px;
        }

        .join-button:hover {
          background: linear-gradient(120deg, #e0c3fc 0%, #8ec5fc 100%);
          text-decoration:none;
        }
    </style>

<div class="logo">
    <img src="https://s2.loli.net/2024/06/07/7vdFaYn3gSL2Csf.png" alt="HASHTEAM Logo" width="100" height="100">
    <h1><strong>HASHTEAM</strong></h1>
</div>

<div class="container">
  <div class="about">
    <h2>关于我们</h2>
    <p>HASHTEAM是由山东大学一群对网络空间安全感兴趣的年轻人组成的兴趣团体，团队成员研究方向包括但不限于软硬件安全，网络攻防，人工智能安全，区块链安全。</p>
    <p>除积极参与国内外泛CTF类比赛外,团队成员还进行安全工具开发，参与护网行动等活动。</p>
    <p>在学院的大力支持下，我们参加了许多全国性比赛如全国大学生信息安全竞赛创新能力实践赛(ciscn)、网鼎杯以及世界性比赛如 defcon，在各项比赛中取得较优异的成绩，以新人的姿态在全国高校中崭露头角。</p>

  </div>

  <div class="skills">
    <h2>技能</h2>
    <svg viewBox="-5 0 120 80" xmlns="http://www.w3.org/2000/svg">
      <!-- 柱状图 -->
      <rect x="30" y="10" width="80" height="9" fill="#007bff" />
      <rect x="30" y="22" width="75" height="9" fill="#28a745" />
      <rect x="30" y="34" width="60" height="9" fill="#dc3545" />
      <rect x="30" y="46" width="65" height="9" fill="#ffc107" />
      <rect x="30" y="58" width="55" height="9" fill="#17a2b8" />
      <!-- 标签 -->
      <text x="20" y="17" text-anchor="end" font-size="6" font-weight="bold">Crypto</text>
      <text x="20" y="29" text-anchor="end" font-size="6" font-weight="bold">Pwn</text>
      <text x="20" y="41" text-anchor="end" font-size="6" font-weight="bold">Web</text>
      <text x="20" y="53" text-anchor="end" font-size="6" font-weight="bold">Reverse</text>
      <text x="20" y="65" text-anchor="end" font-size="6" font-weight="bold">Misc</text>
    </svg>
  </div>
</div>

<div class="container2">
  <div class="history">
    <h2>发展历程</h2>
      <div class="timeline">
        <div class="event">
          <span>2020年</span>
          <span>HASHTEAM成立</span>
        </div>
        <div class="event">
          <span>2022年</span>
          <span>获国赛二等奖</span>
        </div>
        <div class="event">
          <span>2024年</span>
          <span>第一次独立组织校赛</span>
        </div>
        <div class="event">
          <span>2024年</span>
          <span>战队成员突破20人</span>
        </div>
      </div>
    </div>
    
  <div class="achievements">
    <h2>成就</h2>
    <ul>
      <li>第十五届全国大学生信息安全竞赛（创新实践能力赛）二等奖</li>
      <li>第七届蓝帽杯总决赛决赛二等奖</li>
      <li>第四届“长城杯”网络安全大赛暨京津冀网络安全技能竞赛初赛赛区第一，决赛国二</li>
      <li>第十八届全国大学生信息安全竞赛（作品赛）一等奖</li>
      <li>第十八届全国大学生 信息安全竞赛（创新实践能力赛）暨第二届“长城杯”铁人三项赛（防护赛）赛半决赛一等奖，决赛三等奖</li>
      <li>第二届“熵密杯” 全国一等奖</li>
      <li>第十七届全国大学生信息安全竞赛（创新实践能力赛）半决赛三等奖</li>
      <li>······</li>
    </ul>
  </div>
</div>


<div class="container3">
  <div class="about">
    <h2>什么是CTF？</h2>
    <p>CTF(Capture The Flag)是网络安全技术人员之间进行技术竞技的一种比赛形式，主要包括解题模式 (Jeopardy)和攻防模式(Attack & Defense)，</p>
    <p>传统 CTF 竞赛涵盖了⌈Web 网络攻防、Re 逆向工程、Pwn 二进制漏洞利用、Crypto 密码攻击、Mobile 移动安全以及、Misc安全杂项⌋等多种类别，新兴的安全问题如区块链安全、Ai对抗、自动写驶安全、数据安全、邮件安全等也开始逐渐成为进入CTF 赛事的范畴。</p>
  </div>

  <div class="about">
    <h2>你会得到什么？</h2>
    <p>1."做开发要刷Leetcode，搞安全要打CTF。"参加CTF比赛是进入网络安全行业很好的成长途径，CTF 赛题具有与时俱进的特点，新洞新方法层见不鲜，能够激励参赛选手跟进时下更新知识，「极大地提升学生的学习能力和安全实战能力。」</p>
    <p>2.在「安全人员招聘」中，有CTF经历也普遍成为「加分项」，成为进入「大厂」的敲门砖。</p>
    <p>3.此外，相关重要赛事已经列入学院「研究生推免」资格赛事名单。</p>
    <p>4.会有很多跟学院教授交流的机会，能够接触更多让你积累经验的项目，平时去参加比赛也可以(公费旅游)报销!</p>
  </div>
</div>





<div class="container">
  <div class="join-us">
    <h2>加入我们</h2>
    <p>只要你是山东大学的学生，任何年级，任何专业，都欢迎加入我们！</p>
    <a href="https://qm.qq.com/q/W4Lhi8dPaI" class="join-button">联系我们</a>
  </div>
</div>
