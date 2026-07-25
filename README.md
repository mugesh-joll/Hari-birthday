<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<title>Birthday Surprise</title>

<style>
body{
    margin:0;
    font-family:Arial,sans-serif;
    background:linear-gradient(135deg,#ff6ec4,#7873f5);
    display:flex;
    justify-content:center;
    align-items:center;
    height:100vh;
    text-align:center;
    color:white;
}

.container{
    padding:20px;
}

.gift{
    font-size:120px;
    animation:bounce 1s infinite;
}

button{
    padding:15px 30px;
    font-size:20px;
    border:none;
    border-radius:10px;
    cursor:pointer;
}

#message{
    display:none;
    font-size:40px;
    margin-top:20px;
    animation:zoom 1s;
}

@keyframes bounce{
    50%{transform:translateY(-15px);}
}

@keyframes zoom{
    from{transform:scale(0);}
    to{transform:scale(1);}
}
</style>
</head>

<body>

<div class="container">

<div id="giftArea">
<div class="gift">🎁</div>
<br>
<button onclick="openGift()">Open Gift</button>
</div>

<div id="message">
🎉 Happy Birthday Hariprabha! 🎂
</div>

</div>

<script>
function openGift(){
document.getElementById("giftArea").style.display="none";
document.getElementById("message").style.display="block";
}
</script>

</body>
</html>
