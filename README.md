<!DOCTYPE html>
<html lang="en">
<head>
	<meta charset="UTF-8">
	<title>YerevanBox</title>
	<link rel="stylesheet" href="CSS/main.css">
</head>
<body>
	<header>
		<div id="logo" onclick="slowScroll('#top')">
			<span>YerevanBox</span>
		</div>
		<div id="about">
			<a href="index.html" title="Гланая страница" onclick="slowScroll('index.html')">Главная страница</a>
			<a href="#" title="Что может выпасть с ящиков" onclick="slowScroll('#main')">Призы</a>
			<a href="faq.html" onclick="slowScroll('faq.html')" title="Ответы на вопросы">FAQ</a>
		</div>
	</header>

	<div id="top">
		<div>
			<h1>Чтобы покупать бокс жми на неё!</h1>
		
			<div class="img">
				<img class="btn" src="https://static.thenounproject.com/png/566051-200.png" alt="">
			</div>
			<div class="img">
				<img class="btn" src="https://static.thenounproject.com/png/566051-200.png" alt="">
			</div>
		</div>
			<span class="box__text">Бокс за 4000 Армянских драм</span>
			<span class="box__text">Бокс за 8000 Армянских драм</span>
	</div>

	
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.5.1/jquery.min.js"></script>
	
	<script>
		function slowScroll(id) {
			$('html, body').animate({
				scrollTop: $(id).offset().top
			}, 500)
		}

		$(document).on("scroll", function () {
			if($(window).scrollTop() === 0)
				$("header").removeClass("fixed");
			else
				$("header").attr("class", "fixed")
		});
	</script>


</body>
</html>
