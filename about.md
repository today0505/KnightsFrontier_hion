---
layout: default
title: 소개
permalink: /about/
---

<section class="cat-head">
  <div>
    <p class="label"><i class="note-ico"></i>about.txt</p>
    <h1 class="glitch">About</h1>
  </div>
</section>

<div class="about-grid">
  <aside class="about-side note">
    {% include note-top.html file="profile.txt" nomenu=true %}
    <div class="note-body">
      <div class="avatar">
        {% assign photo = site.static_files | where: "path", "/assets/img/profile.jpg" | first %}
        {% if photo %}
          <img src="{{ photo.path | relative_url }}" alt="hion 프로필 사진">
        {% else %}
          <span>hion</span>
        {% endif %}
      </div>

      <p class="side-label">LEARNING SECURITY</p>
      <p class="side-name">원미혜</p>
      <p class="side-nick">@광운대_원미혜(hion)</p>
      <p class="side-nick">소속: 광운대학교</p>

      <div class="side-block">
        <p class="side-label">INTERESTS</p>
        <div class="side-tags"><span>미정</span></div>
      </div>

      <div class="side-block">
        <p class="side-label">ONE LINE</p>
        <p class="side-quote">보안에 대해 아는 것은 적지만, 열심히 배우겠습니다! 잘 부탁드립니다!!</p>
      </div>

      <p class="side-links"><a href="https://github.com/{{ site.github }}" target="_blank" rel="noopener">→ GitHub</a></p>
    </div>
    {% include note-status.html %}
  </aside>

  <div class="about-main content">
    <h2>이 블로그에서 하는 일</h2>
    <p>
      배우는 과정과 활동을 꾸준히 기록합니다.<br>
      CTF 풀이, 버그 바운티 도전기, 읽은 논문, 참가한 공모전과 자격증 준비 과정을
      카테고리별로 정리합니다.
    </p>
    <h2>연락</h2>
    <ul>
      <li>GitHub: <a href="https://github.com/{{ site.github }}" target="_blank" rel="noopener">github.com/{{ site.github }}</a></li>
    </ul>
  </div>
</div>
