---
title: 跳转中...
permalink: /x/download
---

跳转中....

---

[主页](https://cdr-today.github.io/intro/download.html)

<script>
export default {
  mounted () {
    import('./lib-that-access-window-on-import').then(module => {
      var u = window.navigator.userAgent;
      if (/android/i.test(u)) {
          window.location.href = 'https://ct-1253442844.cos.ap-shanghai.myqcloud.com/apk/cdr.today.apk'
      } else if (/iPad|iPhone|iPod/.test(u) && !window.MSStream) {
          window.location.href = 'https://testflight.apple.com/join/rZzzQmPb'
      } else {
          window.location.href = '/download';
      }
    })
  }
}
</script>
