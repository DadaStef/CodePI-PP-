<!DOCTYPE html>
<!--HTML Code-->
<head>
	<title>PWA vježba</title>

    <meta charset="UTF-8" />
    <style>
        
    </style>
</head>
<body>
	<form action ="formula.php" method="get">
        Unesite stranice pravokutnika: <br />
        a: <input type="text" name="stranicaA" /><br />
        b: <input type="text" name="stranicaB" /><br>
       
			<input type="submit" name="submit" value="Pošalji" />

	</form>
</body>
</html>

<?php
/*formula.php / PHP Code */
$strA = $_GET['stranicaA'];
$strB = $_GET['stranicaB'];

function povrsina($privA, $privB){
    $pov = $privA * $privB;
    echo "Površina pravokutnika je $pov";
}
povrsina($strA, $strB);
?>
