# JavaScript--DOM1
<!DOCTYPE HTML>
<html>
<head>
<meta http-equiv="Content-Type" Content="text/html; charset=utf-8" />
<title>javascript</title>
<style type="text/css">
body{font-size:12px;}
#txt{
    height:400px;
    width:600px;
	border:#333 solid 1px;
	padding:5px;}
p{
	line-height:18px;
	text-indent:2em;}
</style>
</head>
<body>
  <h2 id="con">JavaScript课程</H2>
  <div id="txt"> 
     <h5>JavaScript为网页添加动态效果并实现与用户交互的功能。</h5>
        <p>1. JavaScript入门篇，让不懂JS的你，快速了解JS。</p>
        <p>2. JavaScript进阶篇，让你掌握JS的基础语法、函数、数组、事件、内置对象、BOM浏览器、DOM操作。</p>
        <p>3. 学完以上两门基础课后，在深入学习JavaScript的变量作用域、事件、对象、运动、cookie、正则表达式、ajax等课程。</p>
  </div>
  <form>
  <!--当点击相应按钮，执行相应操作，为按钮添加相应事件-->
    <input type="button" value="改变颜色" onclick="changecolor()">  
    <input type="button" value="改变宽高" onclick="changeheight()" >
    <input type="button" value="隐藏内容" onclick="changehide()">
    <input type="button" value="显示内容" onclick="changedisplay()">
    <input type="button" value="取消设置" onclick="rconfirm()">
  </form>
  <script type="text/javascript">
//定义"改变颜色"的函数
    function changecolor(){
      document.getElementById("txt");
      txt.style.color="red";
      txt.style.backgroundColor="gray";
    }

//定义"改变宽高"的函数
    function changeheight(){
      document.getElementById("txt");
      txt.style.width="500px";
      txt.style.height="600px";
    }

//定义"隐藏内容"的函数
    function changehide(){
      document.getElementById("txt");
      txt.style.display="none";
    }

//定义"显示内容"的函数
    function changedisplay(){
      document.getElementById("txt");
      txt.style.display="block";
    }

//定义"取消设置"的函数
     function rconfirm(){
      var mymessage=confirm("是否取消设置？")
      if(mymessage="true")
      {
          document.getElementById("txt");
           txt.style="null";
           
      }
      else{}
    }


  </script>
</body>
</html>
