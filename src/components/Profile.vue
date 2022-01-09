<template>
  <div id="profile">
    <div id="sub_title">[ ABOUT ME ]</div>
    <div id="profile-container">
      <div class="profile-info">
        <div class="profile-title"><span>이름</span></div>
        <div>박동현</div>
      </div>
      <div class="profile-info">
        <div class="profile-title"><span>생년월일</span></div>
        <div>97.06.02</div>
      </div>
      <div class="profile-info">
        <div class="profile-title"><span>전화번호</span></div>
        <div>010-7608-1413</div>
      </div>
      <div class="profile-info">
        <div class="profile-title"><span>이메일</span></div>
        <div>tjswk70000@naver.com</div>
      </div>
      <div class="profile-info">
        <div class="profile-title"><span>학교/전공</span></div>
        <div>한국성서대학교</div>
        <div>컴퓨터소프트웨어학과</div>
      </div>
      <div class="profile-info">
        <div class="profile-title"><span>희망 근무지</span></div>
        <div>서울</div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
#profile {
  text-align: center;
  color: #545454;
}
#sub_title {
  padding-top: 60px;
  margin-bottom: 60px;
  margin-left: auto;
  margin-right: auto;
  font-weight: 900;
  font-size: 3rem;
}
#profile-container {
  font-weight: 500;
  font-size: 1.5rem;
  display: inline-block;
  display: flex;
  flex-flow: row wrap;
}
.profile-info {
  margin-bottom: 30px;
  width: 33.3333%;
}
.profile-title {
  margin-bottom: 20px;
  font-weight: 800;
}
.profile-title span {
  border-bottom: 1px solid;
}
@media (max-width: 990px) {
  .profile-info {
    width: 50%;
  }
}
@media (max-width: 600px) {
  .profile-info {
    width: 100%;
  }
}
</style>
