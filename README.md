<!DOCTYPE html>
<html lang="hu">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Php 1</title>
</head>
<body>
    <?php
        echo '<p>Ezt a PHP írta.</p>';
        echo("echo zárójellel");
        print "<br>print eredménye";
        print("<br>print zárójellel");
        var_dump($GLOBALS);
        //konstans
        echo '<br>';
        define("GREETING","Hello you! How are you today?");
        echo constant("GREETING");

        $szoveg1 = 'Egykor'; 
        $szoveg2 = "végzek.";
        //Az összefűzés jele php-ban a pont
        echo "A két szöveg együtt: ".$szoveg1."+".$szoveg2;
        echo "A két szöveg együtt: $szoveg1 $szoveg2";

        //azu idézőjelek nem egyformák!
        echo '<br>A két szöveg együtt: $szoveg1 $szoveg2';

        //működik a rövid operátor itt is
        $szoveg8 = "Szép";
        $szoveg8 .=" napot!" ;
        echo "<br>$szoveg8";




        echo pow(2.0, 1023);
        $tort1 = 3.56;
        $tort2 = 3.44;
        $eredmeny =  $tort2 +  $tort1;
        echo "<br>A két szám összege: $eredmeny";
        echo gettype($eredmeny);


        //logikai típusok
        echo '0:        '.(boolval(0) ? 'true' : 'false')."\n";
        echo '42:       '.(boolval(42) ? 'true' : 'false')."\n";
        echo '0.0:      '.(boolval(0.0) ? 'true' : 'false')."\n";
        echo '4.2:      '.(boolval(4.2) ? 'true' : 'false')."\n";
        echo '"":       '.(boolval("") ? 'true' : 'false')."\n";
        echo '"string": '.(boolval("string") ? 'true' : 'false')."\n";
        echo '"0":      '.(boolval("0") ? 'true' : 'false')."\n";
        echo '"1":      '.(boolval("1") ? 'true' : 'false')."\n";
        echo '[1, 2]:   '.(boolval([1, 2]) ? 'true' : 'false')."\n";
        echo '[]:       '.(boolval([]) ? 'true' : 'false')."\n";
        echo 'stdClass: '.(boolval(new stdClass) ? 'true' : 'false')."\n";


        //tömbök
        $a = array("red", "green", "blue");
        //print_r($a);

        $tomb0 = array(1,2,3,4,5);
        $tomb1 = array();
        $tomb2[0] = "Ady Endre";
        $tomb2[1] = "József Attila";
        $tomb3 = ["Milan Kundera", "Hermann Hesse"];
        //Hozzáfűzés kétféleképpen:
        $tomb2[] = "Tóth Árpád";
        array_push($tomb2, "Tóth Árpád");
        //Lista elemszáma:
        $elemSzam = count($tomb2);
        //Listák összeillesztése:
        $tomb4 = array_merge($tomb2, $tomb3);



    ?>
</body>
</html>
