<template>
  <div>
    <p>Naver Login Access Pages</p>
  </div>
</template>

<script>
export default {
  mounted() {
    new window.naver_id_login("Tf_9l86UixTtfzNYj2sS", "http://localhost:8080/app.vue");
    console.log("access token", naver_id_login.getAccessToken()); // 정상적 로그인이 된 경우 access token값 출력
  },
};
</script>