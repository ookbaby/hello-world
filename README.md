<html>
	<head>
		<title></title>
		<meta charset="UTF-8"/>
		<script src="test.js" type="text/javascript" charset="utf-8"></script>
		<script type="text/javascript" charset="utf-8">
			function whoise () {
				var e;
				e = document.getElementsByClassName("classA");
				e = document.getElementsByTagName("div");
				e = document.getElementById("d1");
				e.setAttribute("align","center");
				e.setAttribute("data-test","2");
				e.style.fontFamily="微软雅黑";
				e.style.backgroundImage="url(img/HBuilder.png)";
				switch (e.style.display){
					case "-webkit-box":
						break;
					default:
						break;
				}
				if (e.getAttribute("class")!="classA") {
					e.className="classA";
				}
				e.innerHTML="<font color='#CCCCCC'></font>";
				e = document.getElementById("a1");
				e.href="#a1";
				e.target="_blank";
				e = new Image();
				e.src = "img/HBuilder.png";
				e = window.indexedDB || window.webkitIndexedDB || window.msIndexedDB || window.mozIndexedDB;
				if (typeof(e)!="undefined") {
					e.open("test");
				}
				var head = document.getElementsByTagName("head")[0];
				with (head){
					var l= lastElementChild;
					removeBehavior(l);
				}
				e = document.createElement("link");
				e.rel="stylesheet";
				e.type="text/css";
				e.href="test.css";
				head.appendChild(e);
				var ss="e is ";
				if (e.getAttribute('data-test')==null) {
					ss=ss+e.outerHTML;
				} else{
					ss=ss+"unknow";
				}
				alert(ss)
			}
			addEventListener("DOMContentLoaded",function () {
				finishLesson(l)
			})
		</script>
		<style type="text/css">
			body{
				text-align: center;
				-webkit-user-select: none;
			}
			input[type=button]{
				width: 90px;				
			}
			ul{display: none;
			}
			#d1{
				font-family: "微软雅黑";
				background-image: url(img/HBuilder.png);
				
			}
		</style>
		<link rel="stylesheet" type="text/css" href="test.css"/>
	</head>
	<body>
		<img src="img/HBuilder.png"/>
		<br />
		<div id="d1" class="classA" data-test = "1"></div>
		<a href="#a1" id="a1"></a>
		<ul>
			<li></li>
		</ul>
	<nav>&nbsp;</nav>
	<input type="button" name="" id="" value="who is e" onclick="whoise()" />
	</body>
</html>
