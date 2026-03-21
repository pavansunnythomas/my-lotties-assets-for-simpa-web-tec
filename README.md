# my-lotties-assets-for-simpa-web-tec

This a static server for loading assets,

in the head tag of HTML add this:

` <script src="https://unpkg.com/lottie-web@5.12.2/build/player/lottie.min.js"></script> `

In the reqired place add this:

```
<div class="lottie-wrapper">
  <div id="lottie-loader"></div>
</div>

<style>
.lottie-wrapper {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
}

#lottie-loader {
  width: 200px;
  height: 200px;
}
</style>

<script>
document.addEventListener("DOMContentLoaded", function () {
  if (!window.lottie || typeof lottie.loadAnimation !== "function") return;

  lottie.loadAnimation({
    container: document.getElementById("lottie-loader"),
    renderer: "svg",
    loop: true,
    autoplay: true,
    path: "https://pavansunnythomas.github.io/my-lotties-assets-for-simpa-web-tec/lottie-assets/lottie/Write.json"
  });
});
</script>

```

### Available assests:
- https://pavansunnythomas.github.io/my-lotties-assets-for-simpa-web-tec/lottie-assets/lottie/Successfully_done.json
- https://pavansunnythomas.github.io/my-lotties-assets-for-simpa-web-tec/lottie-assets/lottie/Message_Sent.json
- https://pavansunnythomas.github.io/my-lotties-assets-for-simpa-web-tec/lottie-assets/lottie/Write.json
