
<!DOCTYPE html>
<!-- saved from url=(0028)http://loveyue2.sinaapp.com/ -->
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en">

	<head>
		<meta http-equiv="Content-Type" content="text/html; charset=UTF-8">
		<title>Our Love Story</title>

		<style type="text/css">
			@font-face {
				font-family: digit;
				src: url('digital-7_mono.ttf') format("truetype");
			}
		</style>
		<link href="1_files/default.css" type="text/css" rel="stylesheet">
		<script type="text/javascript" src="1_files/jquery.js"></script>
		<script type="text/javascript" src="1_files/garden.js"></script>
		<script type="text/javascript" src="1_files/functions.js"></script>

	</head>

	<body>
		<!-- 浮动广告代码开始 -->
		<div id="ShowAD" style="position: absolute; z-index: 100; top: 159px; left: 15px;">
			<div style="width:150px;height:18px;font-size:14px;font-weight:bold;text-align:center;CURSOR: hand;" onclick="closead();">
				<font color="ff0000">关闭</font>
			</div>
			<a href="http://loveyue1.sinaapp.com/love/index.html" target="_blank" title="title" onclick="closead();">
				<img border="0" alt="alt" src="1_files/bg.png" style="width: 150px;height: 203px"></a>
		</div>
		<script>
			var bodyfrm = (document.compatMode.toLowerCase() == "css1compat") ? document.documentElement : document.body;
			var adst = document.getElementById("ShowAD").style;
			adst.top = (bodyfrm.clientHeight - 530 - 22) + "px";
			adst.left = "15px";

			function moveR() {
				adst.top = (bodyfrm.scrollTop + bodyfrm.clientHeight - 530 - 22) + "px";
				adst.left = "15px";
			}
			setInterval("moveR();", 400);

			function closead() {
				adst.display = 'none';
			}
		</script>
		<!-- 浮动广告代码结束 -->
		<div id="mainDiv">
			<div id="content" style="width: 1110px; height: 625px; margin-top: 43px; margin-left: 213px;">
				<div id="code" style="margin-top: 112.5px;">
					<span class="comments">我的爱人</span><br>
					<span class="space"><span class="comments">我会牵着你的手，走到我们满头白发的那一天</span><br>
					<span class="space"><span class="comments">我会守护你生命里的精彩，并陪伴你一路精彩下去。</span><br>
					<span class="space"><span class="comments">你的幸福快乐，是我一生的追求。</span><br>
					<span class="space">我会每一天带着笑脸，和你说早安，<br>
				<span class="space">我会每一晚与你道声晚安再入梦</span></span>
					</span>
					</span>
					</span>
				</div>
				<div id="loveHeart">
					<canvas id="garden" width="670" height="625"></canvas>
					<div id="words" style="position: absolute; top: 238px; left: 723px;">
						<div id="messages" style="opacity: 0.0160225; display: block;">
							月,我爱你！
							<div id="elapseClock"><span class="digit">2641</span> days <span class="digit">20</span> hours <span class="digit">50</span> minutes <span class="digit">46</span> seconds</div>
						</div>
						<div id="loveu">
							Love u forever and ever.<br>
							<div class="signature">- wuxia2001</div>
						</div>
					</div>
				</div>
			</div>

		</div>
		<script type="text/javascript">
			var offsetX = $("#loveHeart").width() / 2;
			var offsetY = $("#loveHeart").height() / 2 - 55;
			var together = new Date();
			together.setFullYear(2010, 10, 2);
			together.setHours(20);
			together.setMinutes(0);
			together.setSeconds(0);
			together.setMilliseconds(0);

			if(!document.createElement('canvas').getContext) {
				var msg = document.createElement("div");
				msg.id = "errorMsg";
				msg.innerHTML = "Your browser doesn't support HTML5!<br/>Recommend use Chrome 14+/IE 9+/Firefox 7+/Safari 4+";
				document.body.appendChild(msg);
				$("#code").css("display", "none")
				$("#copyright").css("position", "absolute");
				$("#copyright").css("bottom", "10px");
				document.execCommand("stop");
			} else {
				setTimeout(function() {
					startHeartAnimation();
				}, 5000);

				timeElapse(together);
				setInterval(function() {
					timeElapse(together);
				}, 500);

				adjustCodePosition();
				$("#code").typewriter();
			}
		</script>

	</body>

</html>
