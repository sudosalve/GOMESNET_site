<?php
system("clear");
date_default_timezone_set('Africa/Johannesburg');
$date = date("h:i:a");
echo "──────────────────────────────────\n";
echo "\033[1;33m⚠️SCANNER SÓ VAI FUNCIONAR\n\033[1;33mCOM OS DADOS MÓVEIS DO SEU CHIP⚠️\n\033[1;31m🚫COM WIFI NÃO PASSARÁ DESSA PARTE🚫\n";
echo "──────────────────────────────────\n";
$b=readline("\033[1;34mNOME DO SEU ARQUIVO TXT\n:");
$menu = "\033[1;97m[\033[1;36m1\033[m]awselb/2.0              
\033[1;97m[\033[1;36m2\033[m]xneelo                   
\033[1;97m[\033[1;36m3\033[m]cloudflare               
\033[1;97m[\033[1;36m4\033[m]cloudfront               
\033[1;97m[\033[1;36m5\033[m]Apache                   
\033[1;97m[\033[1;36m6\033[m]Apache/2                 
\033[1;97m[\033[1;36m7\033[m]nginx/1.18               
\033[1;97m[\033[1;36m8\033[m]nginx/1.19               
\033[1;97m[\033[1;36m9\033[m]nginx/1.20.1             
\033[1;97m[\033[1;36m10\033[m]nginx/1.25.0            
\033[1;97m[\033[1;36m11\033[m]Para qualquer versão do nginx
\033[1;33mMelhor opção para nginx ~ \033[1;37mé versão 1.20.1 \n";

#################END BANNER##################


#################ONLINE SWITCH##################

$ch = curl_init();
  curl_setopt($ch, CURLOPT_URL, "http://ip-api.com/json/copvps.duckdns.org");
  curl_setopt($ch, CURLOPT_RETURNTRANSFER, 1);
  curl_setopt($ch, CURLOPT_HTTP_VERSION,CURL_HTTP_VERSION_1_1);
  curl_setopt($ch, CURLOPT_POST, 1);
  curl_setopt($ch, CURLOPT_CUSTOMREQUEST,"GET");
  curl_setopt($ch, CURLOPT_PORT,"80");
  curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, true);
  curl_setopt($ch, CURLOPT_TIMEOUT, 15);
  curl_setopt($ch, CURLOPT_ENCODING, '');
  curl_setopt ($ch, CURLOPT_COOKIEJAR, "cookie.txt");
 curl_setopt ($ch, CURLOPT_COOKIEFILE, "cookie.txt");
  $headers = array();
  

$headers[] = 'Content-Type:application/json; charset=utf-8';
$headers[] = 'User-Agent:okhttp/3.12.1';
$headers[] = 'Host:ip-api.com';
$headers[] = 'Connection:Keep-Alive';
$headers[] = 'Accept-Encoding:gzip';

 
  curl_setopt($ch, CURLOPT_HTTPHEADER, $headers);
  $result10 = curl_exec($ch);


$json = json_decode($result10,true);

if($json["org"] == "Google LLC"){
	
system("figlet Offline");

exit;
}else{

###################END SWITCH###################

###################Mini - Menu###################
system("clear");
echo "\033[1;97mTenha certeza que sua lista está correta\n";
echo "──────────────────────────────────\n";
echo "$menu";
echo "────────────────────────────────────────────────\n";
$games = array("don't choose 0", "awselb/2.0", "xneelo", "cloudflare", "cloudfront", "Apache", "Apache/2", "nginx/1.18", "nginx/1.19", "nginx/1.20.1", "nginx/1.25", "nginx");
$a=readline("\033[1;97mAGUARDANDO RESPOSTA:");
$game = trim($games[$a]);
if (!in_array("$game", $games)) {
	system("clear");
	system("figlet Incorrect");
    echo "\033[1;33m Opção invalida❌ usar somente números -> \033[0;31m$a ";
    exit;
}else{
echo "────────────────────────────────────────────────\n";
echo "\033[0;32mPartil de \033[0;33m$game \033[0;32mBoa sorte!";
sleep(5);
###################END Mini Menu###################

##################STAZ HOME####################
system("clear");
echo $titil="\033[0;33m";

}
###################END HOME####################


#################STAZ EXPLODE###################
$live = 0;
$die = 0;
ini_set('display_errors', 1);
ini_set('max_execution_time', 300);
$listcode = ($b); // where u put your hosts
$codelistlist = file_get_contents($listcode);
$code_list_array = file($listcode);
$code = explode(PHP_EOL, $codelistlist);
$count = count($code);
$i ="0";

echo "\033[1;36m[+]~~~~~~~~~~~~~\033[0;32mTotal Hosts/IP's=\033[0;37m[$count]\033[1;36m~~~~~~~~~~~~[+]\r\n"; //banner to display how many to be checked


//now starting the loop.....
while($i < $count) {
  $percentage = round(($i+1)/$count*100,2);
  
  
$staztrick = explode(" ", $code[$i]);//delim
  $site= trim($staztrick[0]);//in php the count start from 0 so the bot takes the first website in list.txt and trims anything else
  
 #################END EXPLODE###################
 
 
 ###################REQUEST 1###################
 $ch = curl_init();
  curl_setopt($ch, CURLOPT_URL, "https://$site");// site here
curl_setopt($ch, CURLOPT_HEADER, true);    // we want headers
curl_setopt($ch, CURLOPT_NOBODY, true);    // we don't need body
curl_setopt($ch, CURLOPT_RETURNTRANSFER,10); //return 10
curl_setopt($ch, CURLOPT_CUSTOMREQUEST,"GET");//payload request
curl_setopt($ch, CURLOPT_PORT,"443");//request port used
#curl_setopt($ch, CURLOPT_SSL_VERIFYPEER, false);//ssl verify
curl_setopt($ch, CURLOPT_TIMEOUT, 2); // the time req must take
$output = curl_exec($ch); // output of request
$httpcode = curl_getinfo($ch, CURLINFO_HTTP_CODE);//code info

curl_close($ch);


################END REQUEST 1###################


##################RESPONSES#################### 

	#echo "$output\n"; //I like to keep this just to see the output when I'm fixing 
	
	
if(strpos($output, "erver: $game")) {
echo "\033[0;32m[✅] Válido --> \033[0;33m$site \n";
$livee = "hits.txt";//file to be saved to
    $fopen = fopen($livee, "a+"); //auto open the file
    $fwrite = fwrite($fopen, "$game zero rated-> $site\n"); //write on the file 
    fclose($fopen); //close the file 
    $live++;
    
}


else{ //This is if the host is not CloudFlare or doesn't open it will print out this text below
echo "\033[0;34m[🚫️] Inválido -->  \033[0;31m$site\n";
	}
	
$i++;

	}
	
}
