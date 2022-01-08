<template>
  <div>
    <div id="navbar">
      <div>
        <a id="logo" href="#">동현이 포트폴리오</a>

        <ul v-if="width > 900">
          <li>
            <a href="#"><b>메뉴1</b></a>
          </li>
          <li>
            <a href="#"><b>메뉴2</b></a>
          </li>
          <li>
            <a href="#"><b>메뉴3</b></a>
          </li>
          <li>
            <a href="#"><b>메뉴4</b></a>
          </li>
        </ul>
        <span v-else>햄버거 메뉴</span>
      </div>
    </div>

    <div id="hero_header">
      <div class="bg"></div>
      <div class="info">
        <h1>박동현</h1>
        <h1>[웹 개발자 포트폴리오]</h1>
        <h2>안녕하세요</h2>
        <h2>꾸준하고 열정적인 저만의 페이스로</h2>
        <h2>
          어떤 개발자보다 트렌디하고 끊임없이 발전하는 개발자 박동현 입니다.
        </h2>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      width: window.innerWidth,
    };
  },
  mounted() {
    window.addEventListener("resize", this.handleResize);
  },
  methods: {
    handleResize() {
      this.width = window.innerWidth;
    },
  },
};
</script>

<style>
#navbar {
  width: 100%;
  height: 60px;
  overflow: hidden;
  background-color: white;
  text-align: center;
}
#navbar div {
  display: inline-block;
  width: 60%;
}

#logo {
  line-height: 60px;
  padding-left: 30px;
  font-weight: 700;
  font-size: 1.5rem;
  text-decoration: none;
  color: #545454;
  float: left;
}

#logo img {
  vertical-align: middle;
}

ul {
  padding-right: 30px;
  list-style: none;
  margin: 0;
  float: right;
  line-height: 60px;
}

ul li {
  float: left;
  vertical-align: middle;
}

ul li a {
  display: block;
  margin-left: 30px;
  text-decoration: none;
  color: #545454;
  font-size: 1rem;
  font-weight: 700;
  font-family: Helvetica;
}

ul li a:hover {
  background-color: #eeeeee;
}

#hero_header {
  background-image: url("../../public/배경사진.jpg");
  background-size: cover;
  background-position: center center;
  height: 450px;
  text-align: center;
  line-height: 450px;
}

.bg {
  background-color: rgba(0, 0, 0, 0.5);
  width: 100%;
  height: 450px;
  position: absolute;
  top: 60px;
}

#hero_header .info {
  position: relative;
  line-height: normal;
  display: inline-block;
  vertical-align: middle;
  z-index: 1000;
}

#hero_header .info h1 {
  font-size: 36px;
  margin: 0;
  margin-bottom: 13px;
  color: white;
  font-weight: 400;
}

#hero_header .info h2 {
  font-size: 16px;
  margin: 0;
  margin-bottom: 10px;
  color: white;
  font-weight: 400;
}
</style>
