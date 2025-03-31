<!DOCTYPE html>
<html>
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>大猫天下第一帅</title>
</head>
<body>
    <h1 style="text-align: center;">大猫天下第一帅</h1>
    <div style="text-align: center; margin-top: 20px;">
        <button onclick="alert('你很有眼光！')">是的，我赞同</button>
        <button id="noButton" onclick="shrinkButton()">不，我不这么认为</button>
    </div>
    <script>
        function shrinkButton() {
            var btn = document.getElementById("noButton");
            var size = parseInt(window.getComputedStyle(btn).fontSize);
            if (size > 5) {
                btn.style.fontSize = (size - 2) + "px";
            } else {
                btn.style.display = "none";
            }
        }
    </script>
</body>
</html>
