# accordion
accordion menu

<!doctype html>
<html lang="en">
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1">
</head>
<body class="myBg cpapPage">
	<style>
		*{
			margin:0;
			padding:0;
		}
		
		.title{
			height:30px;
			background:#dadada;
			position:relative;
		}
		.content{
			min-height:80px;
			background:#aaaaae;
			display:none;
			position:relative;
		}
		.content > .title{
			background:#5d7792;
		}
		.linkBtn{
			float:right;
		}
	</style>
	<section>
		<div class="title">Main Title</div>
			<div class="content">
				<div class="title">What is Lorem Ipsum?</div>
					<div class="content"><p>Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type and scrambled it to make a type specimen book.</p></div>
				<div class="title">Inline Title 2</div>
					<div class="content">Inline Content 2</div>
				<div class="title">Inline Title 3</div>
					<div class="content">Inline Content 3</div>
			</div>
		<div class="title">Main Title 2</div>
		<div class="content">Main Content 2</div>
	</section>

	<script src="jquery-2.1.0.min.js"></script>
	<script>
		$('.title').on('click',function(){
			$(this).next().slideToggle();
		});
		
	</script>
</body>
</html>

