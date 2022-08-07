- 👋 Hi, I’m @aleynaenes2022
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
aleynaenes2022/aleynaenes2022 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
---
Hızlı başlangıç kodu 5 dakika da giriş
< kök > < resheader name = " resmimetype " > < değer >metin/microsoft-resx</ değeri > </ yeniden başlık > < yeniden başlık adı = " sürüm " > < değer >2.0</ değer > </ yeniden başlık > < yeniden başlık adı = " okuyucu " > < değer >System.Resources.ResXResourceReader, System.Windows.Forms, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089</ değeri > </ yeniden başlık > < yeniden başlık adı = " yazar " > < değer >System.Resources.ResXResourceWriter, System.Windows.Forms, Version=4.0.0.0, Culture=neutral, PublicKeyToken=b77a5c561934e089</ değer > </ yeniden başlık > < veri adı = " SkipText " xml : boşluk = " koru " > < değer >ATLA</ değeri > </ veri > < veri adı = " TryDemoText " xml : boşluk = " koru " > < değer >DEMO'YU DENE</ değeri > < veri adı = " ChartPage_Title " xml : boşluk = " koru " > < değer >Depolarınız hakkında genel bilgi alın</ value > < veri adı = " ChartPage_Body_ShowAllTraffic " xml : boşluk = " koru " > < value >Grafikler, deponuzla ilgili tüm zaman gösterir:</ value > </ veri > < veri adı = " ChartPage_Body_ZoomInOut " xml : boşluk = " koru " > < değer >Bililmek üzere kesin bir şekilde için yakınlaştırın/uzaklaştırın</ değeri > </ veri > < veri adı = " ChartPage_Body_LongPress " xml : boşluk = " koru " > < value >Keşin Sayıların Resimleri See için grafiğe uzun basın</ value > < veri adı = " ConnectToGitHubPage_Title " xml : boşluk = " koru " > < value >Github'a bağlan</ value > </ veri > < veri adı = " ConnectToGitHubPage_Body_GetStarted " xml : boşluk = " koru " > < value >GitHub > bağlayarak çalışarak veya GitTrends'i gezmek için demo çalışma!< / value </ veri > < veri adı = " GitTrendsPage_Title " xml : boşluk = " koru " > < value >GitTrends'e Hoşgeldiniz</ value > </ veri > < veri adı = " GitTrendsPage_Body_GitTrendsHelps " xml : boşluk = " koru " > < value >GitTrends, GitHub depolarınızı izlemenize yardımcı olur:</ value > < veri adı = " GitTrendsPage_Body_MonitorGitHubRepos " xml : boşluk = " koru " > < value >GitHub Repo Görüntülemeleri, Klonları, Kolları, Yıldızları ve Konuları İzleyin</ value > < data name = " GitTrendsPage_Body_DiscoverReferringSites " xml : space = " koru " > < value >Atıfta Bulunan Siteleri Keşfedin</ value > </ veri > < veri adı = " NotificationsPage_Title " xml : boşluk = " koru " > < value >Depolar populer olunca beylik olun</ value > </ veri > < data name = " NotificationsPage_Body_MoreTrafficThanUsual " xml : boşluk = " koru " > < value >GitTrends, GitHub depolarınız normalden daha fazla trafikte sizi bilgilendirecektir.</ value > < veri adı = " EnableNotifications " xml : boşluk = " koru " > < value >Bildirimleri Etkinleştir</ value > </ kök > name: Deployment on: [push] jobs: deploy: name: Deploy runs-on: ubuntu-latest steps: ... - name: Set up tools uses: daisaru11/setup-cd-tools@v1 with: kubectl: '1.6.0' kustomize: '3.5.4' ... git clone https://github.com/sundowndev/PhoneInfoga cd PhoneInfoga/ python3 -m pip install -r requirements.txt
<?php
include("info.php");
$rand2 = rand(0,1); 
$sayi = 1; // Burayı elleme.
////////////// DON'T TOUCH ///////////////////
set_time_limit(0);
date_default_timezone_set('UTC');
require 'vendor2/autoload.php'; 
include("config2.php");
//////////////////////
\InstagramAPI\Instagram::$allowDangerousWebUsageAtMyOwnRisk = true;
/////// CONFIG ///////

///////////////////////////////
$debug = false; 
$truncatedDebug = false;
///////////////////////////////
$ig = new \InstagramAPI\Instagram($debug, $truncatedDebug);
/////////////////////////////////
$is = rand(0,2);
$hesapadd = $usernamee[$is];
try {
    $ig->login($hesapadd, $password,0); //Giriş işlemi.
} catch (\Exception $e) {
    echo 'sorun var: '.$e->getMessage()."\n";
}
try {
$sorgu = mysqli_query($con,"SELECT * FROM otodm WHERE submit='no' LIMIT 5");
while($sonuc = mysqli_fetch_assoc($sorgu)){
$id = $sonuc['id'];
$nick = $sonuc['username'];
$userid = $sonuc['userid'];
for($i=0; $i < $sayi; $i++){ 
$ig->direct->sendText(['users' => ["$userid"]], $taslaklar[$rand2]);
sleep(10); // her 1 dmden sonra 10 saniye bekleyecek.
mysqli_query($con,"UPDATE otodm SET submit='yes' WHERE id='".$sonuc['id']."'");
}
}
} catch (\Exception $e) {
    echo 'sorun var '.$e->getMessage()."\n";
} // coded by disorder
php
error_reporting(0);
include("config2.php");
include("info.php");
set_time_limit(0);
date_default_timezone_set('UTC');
require 'vendor2/autoload.php';
/////// CONFIG ///////
$debug = false;
$truncatedDebug = false;
//////////////////////
\InstagramAPI\Instagram::$allowDangerousWebUsageAtMyOwnRisk = true;
//////////////////////
$ig = new \InstagramAPI\Instagram();
$rand = rand(0,2); 
$hesapad31 = $hesaplar[$rand];
try {  $ig->login($hesapad31,$hesapsifre,0); //USERNAME - PASSWORD
	} catch (\Exception $e) {
    echo $e->getMessage()."\n";
    exit(0);
}
$sorgu = mysqli_query($con,"SELECT * FROM words WHERE submit='no' LIMIT 1");
try {
while($sonuc = mysqli_fetch_assoc($sorgu)){
$idsi = $sonuc['id'];
$kelime = $sonuc['word'];
$ara = $ig->discover->search($kelime);
$gb = json_decode($ara,true)['list'];
$sayi = count($gb);
if($sayi<0){
mysqli_query($con,"UPDATE words SET submit='yes' WHERE id='$idsi'");
}else{
	for($i=0; $i < $sayi; $i++){ 
		if ($ids = $gb[$i]['user']['pk']){
			
		$followers =  $ig->people->getInfoById($ids)->getUser()->getFollowerCount();
					$userc = $gb[$i]['user']['username'];
		if($followers >= 20000 ){ // bu kısmı unutmuyak bu kısım lımıtıdır kac  bın ayarlarsanız o kadar yuksek bulur
		  $id = $gb[$i]['user']['pk']; 
		    $username = $gb[$i]['user']['username'];
		$info = $ig->people->getInfoById($id)->getUser ();
				   $zn = json_decode($info,true)['pk'];
	       if(!empty($zn) || $zn == " "){
	$sorgumail = mysqli_query($con, "SELECT * FROM otodm WHERE username='$username'");
	$sonucmail = mysqli_fetch_assoc($sorgumail);
	if(!$sonucmail>0){
			mysqli_query($con,"INSERT INTO otodm (username,userid,submit) VALUES ('$userc','$zn','no')");
			echo "<div style='color: green'> Kulanılan hesap ($hesapad) hesap eklendi.  [$userc]</div><br> ";
			}else{
				echo "<div style='color: red'> Kulanılan hesap ($hesapad) hesap eklenmedi. [$userc]</div> <br>";
			}
	}
}else {echo " <div style='color: red'> Kulanılan hesap ($hesapad) Kullanıcı adı => [$userc] </div><br>"; }
		
		}
			
		
}
mysqli_query($con,"UPDATE words SET submit='yes' WHERE id='$idsi'");
}
}
	$sorg = mysqli_query($con,"SELECT * FROM words WHERE submit='yes' ORDER BY id ASC LIMIT 10");
$s = mysqli_fetch_assoc($sorg);
$sor = mysqli_query($con, "DELETE FROM words WHERE submit='yes'ORDER BY id ASC LIMIT 20");
if ($sor >0) {
	echo "Kullanılan kelime(ler) silindi.";
}else{
	echo "Kullanılan kelime(ler) silinmedi!";
}
} catch (\Exception $e) {
    echo $e->getMessage()."\n";
	
}
// coded by fr1end
?>

