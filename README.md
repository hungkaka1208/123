<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta http-equiv="X-UA-Compatible" content="IE=edge" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<link rel="stylesheet" href="style.css" />

		<link
			rel="stylesheet"
			href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.2.1/css/all.min.css"
			integrity="sha512-MV7K8+y+gLIBoVD59lQIYicR65iaqukzvf/nwasF0nqhPay5w/9lJmVM2hMDcnK1OnMGCdVK+iQrJ7lzPJQd1w=="
			crossorigin="anonymous"
			referrerpolicy="no-referrer"
		/>
		<title>Happy birthday</title>
	</head>
	<body>
		<div class="container">
			<div class="boxcontainer">
				<div class="image">
					<img src="flag.png" alt="" />
				</div>
				<div class="text-happybirthday">
					<img src="texthappy.png" alt="" />
				</div>
				<div class="cake">
					<img src="cake.png" alt="" />
				</div>
				<div class="box-balloon">
					<div class="balloon-item1">
						<img src="balloon.png" alt="" />
					</div>
					<div class="balloon-item1">
						<img src="balloon.png" alt="" />
					</div>
				</div>
				<div class="box-cloud">
					<div class="cloud">
						<img src="cloud.png" alt="" />
					</div>
					<div class="cloud">
						<img src="cloud.png" alt="" />
					</div>
				</div>
				<div class="box-firework">
					<div class="firework">
						<img src="firework.png" alt="" />
						<img src="firework1.png" alt="" id="firework1" />
					</div>
					<div class="firework">
						<img src="firework.png" alt="" />
						<img src="firework1.png" alt="" id="firework1" />
					</div>
				</div>
				<div class="paperCannons">
					<img src="paperCannons1.png" alt="" />
				</div>
				<div class="box-giftbox">
					<img src="giftbox.png" alt="" />
					<img src="giftbox.png" alt="" />
					<img src="giftbox.png" alt="" />
					<img src="giftbox.png" alt="" />
					<img src="giftbox.png" alt="" />
					<img src="giftbox.png" alt="" />
				</div>
				<div class="mail">
					<i class="fa-regular fa-envelope"></i>
				</div>
				<div class="boxcute">
					<div class="cute1">
						<img src="cute.png" alt="" />
					</div>
					<div class="cute2">
						<img src="cute.png" alt="" />
					</div>
				</div>
			</div>
			<div class="boxMail">
				<i class="fa-solid fa-xmark"></i>
				<div class="boxMail-container">
					<div class="card1">
						<div class="userImg">
							<img src="Picture3.jpg" alt="" />
						</div>
						<h3>Happy birthday my lovely</h3>
						<div class="imageCute">
							<img src="cute1.png" alt="" />
						</div>
					</div>
					<div class="card2">
						<div class="card2-content">
							<h3>Gửi Cậu! <br> Công Chúa Của Tớ</h3>

						
							<h2>
								Hôm nay là một ngày vô cùng đặc biệt . Chúc
								cậu có một ngày sinh nhật thật ý nghĩa, vui vẻ vẻ, hạnh phúc bên
								gia đình và bạn bè. Chúc cậu sang tuổi mới lun lun vui vẻ, ngày càng xinh đẹp
								hơn . Tuy tớ không ở gần cậu và có những món quà ý nghĩa đối với cậu nhưng tớ vẫn luôn
								mong muốn những điều tốt đẹp đến với cậu. Tớ chỉ biết dùng vẻ
								đẹp của IT làm quà tặng cậu tuy chỉ là 1 giao diện không phải là 1
								món quà vật chất nhưng tớ mong muốn rằng nó sẽ là 1 món quà ý
								nghĩa, 1 món quà tinh thần nào đó trong ngày đặc biệt của cậu. Và
								cuối cùng chúc cậu cô gái đặc biệt của tớ sinh nhật vui vẻ nha.
								Chúc em tất cả những điều tốt đẹp nhất.Yêu cậu nhiều ❤️❤️
								
							</h2>
							<h3> 💕💕💕💕💕</h3>
							<div class="imageCute2">
								<img src="cute2.png" alt="" />
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
	</body>
	<script>
		document.addEventListener('mousemove', function (e) {
			let body = document.querySelector('body');
			let heart = document.createElement('span');
			let x = e.offsetX;
			let y = e.offsetY;
			heart.style.left = x + 'px';
			heart.style.top = y + 'px';

			let size = Math.random() * 10;
			heart.style.width = 4 * size + 'px';
			heart.style.height = 4 * size + 'px';

			let transformValue = Math.random() * 360;
			heart.style.transform = 'rotate(' + transformValue + 'deg)';

			body.appendChild(heart);

			setTimeout(function () {
				heart.remove();
			}, 1200);
		});

		let mailBox = document.querySelector('.mail');
		let boxmail = document.querySelector('.boxMail');
		var close = document.querySelector('.fa-xmark');
		mailBox.onclick = function () {
			mailBox.classList.toggle('active');
			boxmail.classList.add('active');
		};

		close.addEventListener('click', function () {
			boxmail.classList.remove('active');
		});
	</script>
</html>
