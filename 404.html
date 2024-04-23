<?php
// URL API
$api_url = "https://script.google.com/macros/s/AKfycbyjXkTsLtNT_Bjw2pNceLlr0Xj-pgXsYsl_-Py7cfr3N0YVfH8OqGwlhuaTUKBEpAvS/exec";

// Buat pengaturan permintaan
$options = array(
	'http' => array(
		'header'  => "Content-type: application/json",
		'method'  => 'GET',
	)
);

// Buat konteks permintaan
$context  = stream_context_create($options);

// Lakukan permintaan ke API
$result = file_get_contents($api_url, false, $context);

// Periksa apakah permintaan berhasil
if ($result !== FALSE) {
	// Konversi respons menjadi array asosiatif
	$response = json_decode($result, true);
} else {
	// Permintaan gagal, lakukan penanganan kesalahan di sini
	echo "Permintaan ke API gagal.";
}
$set = $response['data'];
?>
<!DOCTYPE html>
<html>

<head>
	<meta charset="utf-8">
	<meta http-equiv="X-UA-Compatible" content="IE=edge">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>Pengumuman Kelulusan</title>
	<link href="css/bootstrap.min.css" rel="stylesheet">
	<link href="css/jasny-bootstrap.min.css" rel="stylesheet">
	<link href="css/kelulusan.css" rel="stylesheet">
	<style>
		/* general styling */
		:root {
			--smaller: .75;
		}

		* {
			box-sizing: border-box;
			margin: 0;
			padding: 0;
		}

		body {
			margin: 70px 0;
			align-items: center;
			background-color: green;
			/* display: flex; */
			overflow: hidden;
			font-family: -apple-system,
				BlinkMacSystemFont,
				"Segoe UI",
				Roboto,
				Oxygen-Sans,
				Ubuntu,
				Cantarell,
				"Helvetica Neue",
				sans-serif;
		}

		input {
			padding: 5px;
			margin: 5px;
			width: 80%
		}

		.container {
			color: white;
			margin: 0 auto;
			text-align: center;
		}

		h1 {
			font-weight: normal;
			letter-spacing: .125rem;
			text-transform: uppercase;
		}

		li {
			display: inline-block;
			font-size: 1em;
			list-style-type: none;
			padding: 0.5em;
			text-transform: uppercase;
		}

		li span {
			display: block;
			font-size: 3.5rem;
		}

		@media all and (max-width: 768px) {
			h1 {
				font-size: calc(1.7rem * var(--smaller));
			}

			li {
				font-size: calc(1.3rem * var(--smaller));
			}

			li span {
				font-size: calc(4rem * var(--smaller));
			}

			#borderHitungMundur {
				width: 90%
			}

			#borderHasil {
				width: 90%
			}
		}

		.tombol {
			color: black;
			padding: 0px 10px;
			font-size: 1.2em;
			background: #FFB43D;
			cursor: pointer;
			width: fit-content;
			margin: 5px auto;
		}

		#loading {
			width: 100%;
			height: 100%;
			z-index: 999;
			background: black;
			opacity: 0.5;
			top: 0px;
			position: fixed;
			text-align: center;
			color: white;
			display: none;
		}

		.loadingText {
			position: relative;
			top: 70%;
		}

		.sekolah {
			color: #FFB43D;
		}

		#cpr a {
			color: white;
			text-decoration: none;
			font-weight: bold;
		}
	</style>
</head>

<body>
	<div class="container">
		<img src="https://upload.wikimedia.org/wikipedia/commons/9/9a/Kementerian_Agama_new_logo.png" height="100px"></img>
		<h2>Pengumuman Kelulusan <?= htmlspecialchars($set['tahun']); ?></h2>
		<!-- countdown -->
		<div id="borderHitungMundur" style="margin:20px auto;padding:10px;max-width:440px;border:1px solid white;border-radius:5px;">
			<ul>
				<li><span id="hari"></span>hari</li>
				<li><span id="jam"></span>jam</li>
				<li><span id="menit"></span>menit</li>
				<li><span id="detik"></span>detik</li>
			</ul>
		</div>

		<div id="xpengumuman">
			<?php
			if (isset($_POST['submit'])) {
				$data = array(
					'nomor' => $_POST['nomor']
				);

				// URL API
				$api_url = "https://script.google.com/macros/s/AKfycbyINrb034keSD_auUkgYzm3GqcfXQj0zp_3QXL7g8y7RNZJe1tGBNU7Xg7uqYjjQ2XU/exec";

				// Buat pengaturan permintaan
				$options = array(
					'http' => array(
						'header'  => "Content-type: application/json",
						'method'  => 'POST',
						'content' => json_encode($data)
					)
				);

				// Buat konteks permintaan
				$context  = stream_context_create($options);

				// Lakukan permintaan ke API
				$result = file_get_contents($api_url, false, $context);

				// Periksa apakah permintaan berhasil
				if ($result !== FALSE) {
					// Konversi respons menjadi array asosiatif
					$response = json_decode($result, true);
				} else {
					// Permintaan gagal, lakukan penanganan kesalahan di sini
					echo "Permintaan ke API gagal.";
				}
				if ($response['success']) {
					$data = $response['data'];
					// Tampilkan data siswa
					?>
					<table class="table table-bordered">
						<tr>
							<td>Nomor Ujian</td>
							<td><?= htmlspecialchars($data['no_ujian']); ?></td>
						</tr>
						<tr>
							<td>NISN</td>
							<td><?= htmlspecialchars($data['nisn']); ?></td>
						</tr>
						<tr>
							<td>Nama Siswa</td>
							<td><?= htmlspecialchars($data['nama']); ?></td>
						</tr>
						<tr>
							<td>Kelas</td>
							<td><?= htmlspecialchars($data['kelas']); ?></td>
						</tr>
						<tr>
							<td>Rata Rata Nilai AM</td>
							<td><?= htmlspecialchars($data['nilai']); ?></td>
						</tr>
					</table>

				<?php
						if ($data['status'] == 1) {
							echo '<div class="alert alert-success" role="alert"><strong>SELAMAT !</strong> Anda dinyatakan LULUS.</div>';
						} else {
							echo '<div class="alert alert-danger" role="alert"><strong>MAAF !</strong> Anda dinyatakan TIDAK LULUS.</div>';
						}
					} else {
						echo '<div class="alert alert-danger" role="alert">' . $response['message'] . '</div>';
					}
				} else {
					// Tampilkan form input nomor ujian
					?>
				<p>Masukkan nomor ujianmu pada form yang disediakan.</p>

				<form method="post">
					<div class="input-group">
						<input type="text" name="nomor" class="form-control" data-mask="24-13-32-3-0501-9999" placeholder="Nomor Ujian" required>
						<span class="input-group-btn">
							<button class="btn btn-primary" style="top: 2.5px;" type="submit" name="submit">Periksa!</button>
						</span>
					</div>
				</form>
			<?php
			}
			?>

		</div>
	</div><!-- /.container -->

	<footer class="footer">
		<div class="container">
			<p class="text-muted">&copy; <?= htmlspecialchars($set['tahun']); ?> &middot; Tim IT <?= htmlspecialchars($set['sekolah']); ?></p>
		</div>
	</footer>

	<!-- jQuery (necessary for Bootstrap's JavaScript plugins) -->
	<script src="js/jquery.min.js"></script>
	<script src="js/jquery.countdown.min.js"></script>
	<script src="js/bootstrap.min.js"></script>
	<script src="js/jasny-bootstrap.min.js"></script>
	<script type="text/javascript">
		$(document).ready(function() {
			var skrg = Date.now();
			$('#borderHitungMundur').countdown("<?= htmlspecialchars($set['tanggal']); ?>", {
					elapse: true
				})
				.on('update.countdown', function(event) {
					var $this = $(this);
					if (event.elapsed) {
						$("#xpengumuman").show();
						$("#borderHitungMundur").hide();
					} else {
						$('#hari').text(event.strftime('%D'));
						$('#jam').text(event.strftime('%H'));
						$('#menit').text(event.strftime('%M'));
						$('#detik').text(event.strftime('%S'));
						$("#xpengumuman").hide();
					}
				});
		});
	</script>
</body>

</html>