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
    <div class="gallery__specifications">
      <div class="gallery__title">Shoo's Profolio</div>
      <ul class="gallery__tags">
        <li class="gallery__tag">Vue3</li>
        <li class="gallery__tag">Sass 管理樣式結構</li>
        <li class="gallery__tag">API 串接</li>
      </ul>
    </div>

    <iframe
      class="gallery__demo"
      src="https://shooboost.github.io/nice_trip/"
      frameborder="0"
    ></iframe>
  </div>
  <div class="gallery gallery--green">
    <div class="gallery__specifications">
      <div class="gallery__title">Shoo's Profolio</div>
      <ul class="gallery__tags">
        <li class="gallery__tag">Vue3</li>
        <li class="gallery__tag">Sass 管理樣式結構</li>
        <li class="gallery__tag">API 串接</li>
      </ul>
    </div>
    <iframe
      class="gallery__demo"
      src="https://shooboost.github.io/taiwan_bus/"
      frameborder="0"
    ></iframe>
  </div>
  <div class="experience"></div>
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
@keyframes scaleUpAndDown {
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
    animation-name: scaleUpAndDown;
    animation-duration: 5s;
    animation-iteration-count: infinite;
  }
}
.banner--primary {
  background-color: rgb(255, 206, 217);
  color: white;
}

.gallery {
  height: 100vh;
  display: flex;
  padding: 36px 48px;
  box-sizing: border-box;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  @include pad {
    padding: 20px 20px;
  }
  .gallery__specifications {
    display: flex;
    width: 100%;
    justify-content: space-between;
    font-size: 24px;
    @include pad {
      font-size: 14px;
    }

    .gallery__title {
      background-color: #fff;
      padding: 10px 20px;
      border-radius: 20px 20px 0px 0px;
      @include pad {
        padding: 10px;
        border-radius: 16px 16px 0px 0px;
      }
    }
    .gallery__tags {
      display: flex;
    }
    .gallery__tag {
      color: white;
      padding: 10px;
      margin-left: 12px;
      @include pad {
        margin-left: 6px;
      }
    }
  }

  .gallery__demo {
    border-radius: 0px 20px 20px 20px;
    width: 100%;
    height: 100%;
    @include pad {
      border-radius: 0px 16px 16px 16px;
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
}
.gallery--green {
  background-color: rgb(205, 241, 191);
  .gallery__title {
    color: rgba(86, 202, 40, 1);
  }
  .gallery__tag {
    background-color: rgba(86, 202, 40, 0.5);
  }
}
.experience {
  height: 100vh;
  background-color: rgba(255, 200, 0, 0.25);
}
</style>
