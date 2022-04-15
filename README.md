# Lab5web
<!DOCTYPE html>
<html>
<head>
	<title>script untuk melakukan validasi pada isian form</title>
	<link rel="stylesheet" type="text/css" href="style.css">
</head>
<body>
	<center><h2>tugas pemrograman web</h2></center>
	<div class="login">
		<form action="#" method="POST" onSubmit="validasi()">
			<div>
				<label>Nama Lengkap:</label>
				<input type="text" name="nama" id="nama" />
			</div>
			<div>
				<label>Email:</label>
				<input type="email" name="email" id="email" />
			</div>
			<div>
				<label>Alamat:</label>
				<textarea cols="40" rows="5" name="alamat" id="alamat"></textarea>
			</div>
			<div>
				<input type="submit" value="Daftar" class="tombol">
			</div>
		</form>
	</div>
</body>
<script type="text/javascript">
	function validasi() {
		var nama = document.getElementById("nama").value;
		var email = document.getElementById("email").value;
		var alamat = document.getElementById("alamat").value;
		if (nama != "" && email!="" && alamat !="") {
			return true;
		}else{
			alert('Anda harus mengisi data dengan lengkap !');
		}
	}
</script>
<style>
body {
	background: #3498db;
	font-family: sans-serif;
   }
	  
   h2 {
	color: #fff;
   }
	  
   .login {
	padding: 1em;
	margin: 2em auto;
	width: 17em;
	background: #fff;
	border-radius: 3px;
   }
	  
   label {
	font-size: 10pt;
	color: #555;
   }
	  
   input[type="text"],
   input[type="email"],
   textarea {
	padding: 8px;
	width: 95%;
	background: #efefef;
	border: 0;
	font-size: 10pt;
	margin: 6px 0px;
   }
	  
   .tombol {
	background: #3498db;
	color: #fff;
	border: 0;
	padding: 5px 8px;
   }
</style>
</html>
