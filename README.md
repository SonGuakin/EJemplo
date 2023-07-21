<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="Estilos corazon/Corazon.css">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>TE QUIERO MUCHO</title>
</head>

<body>
    <div class="heart"></div>
</body>
</html>
*{
 padding: 0;
 margin: 0;
 box-sizing: border-box;
}

body {
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    background: #222f3e;
    
}
.heart {
    position: relative;
    width: 70px;
    height: 70px;
    background: #ff4757;
    transform: rotate(-45deg);
    box-shadow: -10px 10px 90px #ff4757;
    animation: animate .6s linear infinite;
}
@keyframes animate {
  0% 
    { 
    transform: rotate(-45deg) scale(1.07);
    }
    80% {
        transform: rotate(-45deg) scale(1.0);

    }
    100% {
        transform: rotate(-45deg) scale(0.8);
    }
   }
.heart::before {
    content:'';
    position: absolute;
    top: -50%;
    width: 70px;
    height: 70px;
    background: #ff4757;
    border-radius: 50%;
    box-shadow: 10px 10px 90px #ff4757;
 }

 .heart::after {
    content:'';
    position: absolute;
    right: -50%;
    width: 70px;
    height: 70px;
    background: #ff4757;
    border-radius: 50%;
    box-shadow: 10px 10px 90px #ff4757;
 }
