# Square-to-circle-transformation
......html......
<!DOCTYPE>
<html>
  <head>
     <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <link href="style.css" rel="stylesheet" type="text/css" />
    </head>
<div class="box-circle-transform"></div>
</html>
.....css.....
@-webkit-keyframes square-to-circle {
  0%{
    border-radius: 0 0 0 0;
    transform: rotate(0deg);
    background:violet;
  }
  25%{
    border-radius: 50% 0 0 0;
    transform: rotate(45deg);
    background:#ff4500;
  }
  50%{
    border-radius: 50% 50% 0 0;
    transform: rotate(90deg);
    background:#ffff00;
  }
  75%{
    border-radius: 50% 50% 50% 0;
    transform: rotate(135deg);
    background:#db7093;
  }
  100%{
    border-radius: 50%;
    transform: rotate(180deg);
    background:#ff00ff;
  }
}
body{
  margin:0;
  padding:0;
  background-color: #ffe4e1; 
  height: 100vh;
  width: 100vw;
}
.box-circle-transform{
  margin:auto;
  width: 200px;
  height: 200px;
  background-color: #000080;
  outline: 1px solid transparent;
  -webkit-animation: square-to-circle 3s 2s infinite cubic-bezier(1,.015,.295,1.225) alternate;
  -moz-animation: square-to-circle 3s 2s infinite cubic-bezier(1,.015,.295,1.225) alternate;
  -ms-animation: square-to-circle 3s 2s infinite cubic-bezier(1,.015,.295,1.225) alternate;
  -o-animation: square-to-circle 3s 2s infinite cubic-bezier(1,.015,.295,1.225) alternate;
  animation: square-to-circle 3s 2s infinite cubic-bezier(1,.015,.295,1.225) alternate;
  
  position: relative;
  top: 50%;
  transform: translateY(-50%);
}
