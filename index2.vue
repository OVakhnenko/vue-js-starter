<!DOCTYPE html>
<html>
<head>
    <title>My first Vue app</title>
    <script src="https://unpkg.com/vue"></script>
</head>
<div id="app-2">
  <span v-bind:title="message">
    Наведи курсор на меня пару секунд,
    чтобы увидеть динамически связанное значение title!
  </span>
</div>

<script>
    var app2 = new Vue({
        el: '#app-2',
        data: {
            message: 'Вы загрузили эту страницу: ' + new Date().toLocaleString()
        }
    })
</script>
</body>
</html>