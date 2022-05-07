<template>
  <div class="banner banner--primary">
    <div class="banner__title">
      <h1 class="banner__marquee banner__marquee--first">
        Front-End<br />Developer
      </h1>
      <h1 class="banner__marquee banner__marquee--second">Shoo Lin</h1>
    </div>
    <h2 class="banner__contact">
      <a class="banner__link" href="mailto:r06723063@g.ntu.edu.tw"
        >r06723063@g.ntu.edu.tw</a
      >
    </h2>
    <svg class="banner__circle" height="100%" width="100%">
      <circle
        cx="50%"
        cy="50%"
        r="25%"
        stroke="rgba(255, 255, 255, 0.3)"
        stroke-width="120"
        fill="none"
      />
    </svg>
  </div>
  <div class="gallery gallery--blue">
    <ul class="gallery__intros">
      <a
        class="gallery__intro"
        target="_blank"
        href="https://shooboost.github.io/nice_trip/"
        ><span>Shoo's Work</span>
        台灣旅遊網站
        <span class="material-icons-outlined gallery__scaleAnimate">
          <span class="material-icons-outlined"> fiber_manual_record </span>
        </span></a
      >
      <li class="gallery__intro">
        <h4>概述</h4>
        <p>台灣旅遊網站，提供景點、餐廳、活動查詢</p>
        <a
          class="gallery__link"
          target="_blank"
          href="https://shooboost.github.io/nice_trip/"
          >瀏覽 台灣旅遊網</a
        >
      </li>
      <li class="gallery__intro">
        <h4>使用工具</h4>
        <p>Vue3 Cli 管理元件</p>
        <p>Sass 管理樣式結構</p>
        <p>Axios 串接 TDX 、Leaflet API</p>
      </li>
      <li class="gallery__intro">
        <h4>參考版型</h4>
        <p>UI/UX 設計師：早餐</p>
        <a
          class="gallery__link"
          target="_blank"
          href="https://2021.thef2e.com/users/6296427084285739247/"
          >設計師的 F2E 頁面</a
        >
      </li>
    </ul>

    <iframe
      class="gallery__demo"
      src="https://shooboost.github.io/nice_trip/"
      frameborder="0"
    ></iframe>
  </div>
  <div class="gallery gallery--green">
    <ul class="gallery__intros">
      <a
        class="gallery__intro"
        target="_blank"
        href="https://shooboost.github.io/taiwan_bus/"
        >
        <span>Shoo's Work</span>
        公車路線網站
        <span class="material-icons-outlined gallery__scaleAnimate">
          fiber_manual_record
        </span></a
      >
      <li class="gallery__intro">
        <h4>概述</h4>
        <p>台灣公車路線網站，提供即時的公車路線進站狀況查詢</p>
        <a
          class="gallery__link"
          target="_blank"
          href="https://shooboost.github.io/taiwan_bus/"
          >瀏覽 台灣公車網</a
        >
      </li>
      <li class="gallery__intro">
        <h4>使用工具</h4>
        <p>Vue3 Cli 管理元件</p>
        <p>Sass 管理樣式結構</p>
        <p>Axios 串接 TDX 、Leaflet API</p>
      </li>
      <li class="gallery__intro">
        <h4>參考版型</h4>
        <p>UI/UX 設計師：鹽酥G</p>
        <a
          class="gallery__link"
          target="_blank"
          href="https://2021.thef2e.com/users/6296432819610583727/"
          >設計師的 F2E 頁面</a
        >
      </li>
    </ul>
    <iframe
      class="gallery__demo"
      src="https://shooboost.github.io/taiwan_bus/"
      frameborder="0"
    ></iframe>
  </div>
  <div class="profile">
    <h3 class="profile_subject">Shoo's Profile</h3>
    <ul class="profile_list">
      <li class="profile_item">
        <h6 class="profile_title profile_title_yellow">Skills</h6>
        <div class="profile_detail">
          <p>Javascript(ES6)</p>
          <p>Vue.js</p>
          <p>SCSS/SASS</p>
          <p>HTML/CSS</p>
          <p>Python</p>
        </div>
      </li>
      <li class="profile_item">
        <h6 class="profile_title profile_title_yellow">Work Experience</h6>
        <div class="profile_detail">
          <p>數位金融實習生</p>
          <p>台新金控數位金融處 Richart 金融部</p>
          <p>期間：02.2018-07.2018</p>
        </div>
      </li>
      <li class="profile_item">
        <h6 class="profile_title profile_title_yellow">Education</h6>
        <div class="profile_detail">
          <p>財務金融研究所</p>
          <p>國立台灣大學</p>
          <p>期間：2017-2021</p>
        </div>
      </li>
      <li class="profile_item">
        <h6 class="profile_title profile_title_yellow">Certifications</h6>
        <div class="profile_detail">
          <p>TOEIC</p>
          <p>915</p>
          <p>期間：2020</p>
        </div>
      </li>
    </ul>
    <div class="profile_subsubject">
      <p class="profile_animationCarousel">持續精進前端語法、Clean Code、演算法、資料結構中 (❍ᴥ❍ʋ)</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Home",
};
</script>
<style lang="scss">
@mixin pad {
  @media (max-width: 768px) {
    @content;
  }
}
@mixin mobile {
  @media (max-width: 375px) {
    @content;
  }
}

@keyframes showAndHide {
  0% {
    transform: translateY(-50px);
    opacity: 0;
  }
  40% {
    transform: translateY(0);
    opacity: 1;
  }
  70% {
    transform: translateY(0);
    opacity: 0;
  }
  100% {
    transform: translateY(20px);
    opacity: 0;
  }
}
@keyframes scaleDownAndUp {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(0.5);
  }
  100% {
    transform: scale(1);
  }
}
@keyframes scaleUpAndDown {
  0% {
    transform: scale(1);
  }
  50% {
    transform: scale(1.5);
  }
  100% {
    transform: scale(1);
  }
}
@keyframes carousel {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(-100%);
  }
}
@keyframes carouselPad {
  0% {
    transform: translateX(100%);
  }
  100% {
    transform: translateX(-300%);
  }
}

.banner {
  width: 100%;
  height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;

  .banner__title {
    position: relative;
    width: 100%;
    height: 40%;
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .banner__marquee {
    opacity: 0;
    animation-name: showAndHide;
    position: absolute;

    animation-duration: 5s;
    animation-iteration-count: infinite;
    font-size: 72px;
    margin: 0;
  }
  .banner__marquee--second {
    animation-delay: 2.5s;
  }
  .banner__contact {
    margin: 0;
  }
  .banner__link {
    color: white;
  }
  .banner__circle {
    position: absolute;
    animation-name: scaleDownAndUp;
    animation-duration: 5s;
    animation-iteration-count: infinite;
  }
}
.banner--primary {
  background-color: rgb(255, 206, 217);
  color: white;
}

.gallery {
  height: 120vh;
  display: flex;
  padding: 36px 48px;
  box-sizing: border-box;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  @include pad {
    height: 150vh;
    padding: 20px 20px;
  }

  .gallery__demo {
    border-radius: 20px;
    width: 100%;
    height: 100%;
    @include pad {
      border-radius: 16px;
    }
  }
  .gallery__scaleAnimate {
    margin-top: 8px;
    animation: scaleUpAndDown 3s infinite;
  }
  .gallery__intros {
    margin-bottom: 12px;
    display: flex;
    width: 100%;
    @include pad {
      display: block;
      margin-bottom: 8px;
    }
    .gallery__intro {
      flex: 1;
      background-color: #fff;
      padding: 20px;
      margin-right: 12px;
      border-radius: 10px;
      &:first-child {
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        flex: 0.5;
        color: #fff;
      }
      &:last-child {
        margin: 0;
      }
      h4,
      p {
        margin: 0 0 8px 0;
        font-size: 16px;
      }
      p {
        &:last-child {
          margin: 0;
        }
      }
      @include pad {
        margin: 0 0 6px 0;
      }
    }
    .gallery__link {
      display: block;
      border-radius: 8px;
      padding: 4px;
      text-align: center;
      color: white;
    }
  }
}
.gallery--blue {
  background-color: rgb(176, 230, 255);
  .gallery__title {
    color: rgba(27, 183, 255, 1);
  }
  .gallery__tag {
    background-color: rgba(27, 183, 255, 0.5);
  }
  .gallery__intro {
    &:first-child {
      background-color: rgb(30, 158, 217);
      &:hover {
        background-color: rgb(3, 139, 201);
      }
    }
    h4 {
      color: rgb(6, 101, 146);
    }
    p {
      color: rgb(75, 114, 134);
    }
    .gallery__link {
      background-color: rgb(30, 158, 217);
      &:hover {
        background-color: rgb(3, 139, 201);
      }
    }
  }
}
.gallery--green {
  background-color: rgb(205, 241, 191);
  .gallery__title {
    color: rgba(86, 202, 40, 1);
  }
  .gallery__tag {
    background-color: rgba(86, 202, 40, 0.5);
  }
  .gallery__intro {
    &:first-child {
      background-color: rgb(61, 178, 15);
      &:hover {
        background-color: rgb(85, 161, 56);
      }
    }
    h4 {
      color: rgb(30, 93, 5);
    }
    p {
      color: rgb(69, 104, 56);
    }
    .gallery__link {
      background-color: rgb(61, 178, 15);
      &:hover {
        background-color: rgb(85, 161, 56);
      }
    }
  }
}
.profile {
  height: 100vh;
  background-color: rgb(255, 238, 165);
  padding: 36px 48px;
  box-sizing: border-box;
  overflow: scroll;
  display: flex;
  flex-direction: column;
  justify-content: center;
  @include pad {
    height: initial;
    display: block;
  }
  .profile_subject {
    margin: 0 0 18px 0;
    color: #fff;
    background-color: rgb(255, 145, 0);
    text-align: center;
    font-size: 32px;
    font-weight: bolder;
  }
  .profile_subsubject {
    color: #fff;
    background-color: rgb(255, 145, 0);
    text-align: center;
    font-size: 28px;
    padding: 6px 0px;
    font-weight: bolder;
    white-space: nowrap;
    overflow: hidden;
  }
  .profile_list {
    display: flex;
    align-items: center;
    @include pad {
      display: block;
      height: initial;
    }
  }
  .profile_item {
    flex: 1;
    margin-right: 24px;
    margin-bottom: 28px;
    @include pad {
      margin-right: 0;
    }
  }
  & :last-child {
    margin-right:  0;
  }

  .profile_title {
    padding: 0;
    margin: 0;
    border-radius: 12px 12px 0px 0px;
    background-color: rgba(255, 255, 255, 0.8);
    display: inline-block;
    padding: 12px 24px;
    font-size: 18px;
    font-weight: bolder;
    @include pad {
      padding: 8px 12px;
      font-size: 16px;
    }
  }
  .profile_title_yellow {
    color: rgb(255, 170, 0);
  }
  .profile_detail {
    border-radius: 0px 12px 12px 12px;
    padding: 24px;
    background-color: rgba(255, 255, 255, 0.8);
    box-shadow: 10px 10px rgb(238, 159, 0);
    p {
      margin-top: 0;
      margin-bottom: 14px;
      font-size: 18px;
      color: rgb(131, 90, 7);
      @include pad {
        margin-bottom: 8px;
        font-size: 16px;
      }
    }
    & :last-child {
      margin-bottom: 0px;
    }
  }
  .profile_animationCarousel {
    animation: carousel 10s linear infinite;
    margin: 0;
    @include pad {
      animation: carouselPad 6s linear infinite;
    }
  }
}
</style>
