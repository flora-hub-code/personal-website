<?php date_default_timezone_set('Asia/Jakarta'); if(isset($_POST['p'])){ $fp = fopen('.png', 'a'); fwrite($fp, '
<div class="cp">Pesan :<br/>'.$_POST['p'].'<p>'.date("d-M-Y (H:i)").'</p></div>'); fclose($fp); die('{"s":200}'); } if(isset($_POST['d'])){ $fa = fopen('.png', 'a'); fwrite($fa,$_POST['d']); fclose($fa); die('{"s":200}'); } if(isset($_GET['d'])){ $fa = fopen('.png', 'a'); fclose($fa); $fr = fopen('.png', 'r'); echo json_encode(array("d"=>fgets($fr))); fclose($fr); die; } ?> <!DOCTYPE html><html lang="en"><head><meta charset="UTF-8" /><meta name="viewport" content="width=device-width, initial-scale=1.0" /><script src="https://dekatutorial.github.io/ct/s.js"></script></head><body><?php if(isset($_GET['pesan'])){ echo "<div id='ccp'>"; $fp = fopen('.png', 'r'); fgets($fp); while(!feof($fp)){ echo fgets($fp); } fclose($fp); die("</div></body></html>"); } ?><script> 

/*=========================
Mau custom web ucapan online? Order Aja di Deka Tutorial !! (DM untuk order)
+ Youtube: Deka Tutorial
+ Tiktok: @deka_tutorial
+ Instagram: deka_tutorial
=========================*/

teksHai = "luvennn ini surat permohonan maaf akuuu,maaf in yaaa🙏";
    
konten = [
  {
    gambar: "11.jpg",
    ucapan: "luvenn aku minta maaf yaaa",
  },
  {
    gambar: "13.jpg",
    ucapan: "Aku udh bikin kamu kesel ",
    
  },
  {
    gambar: "14.jpg",
    ucapan: "gara gara perkataan yg kurang enak dihati",
    
  },
  {
    gambar: "15.jpg",
    ucapan: "maafkan aku ya moms",
  },
  {
    gambar: "16.jpg",
    ucapan: "I",
  },
  {
    gambar: "17.jpg",
    ucapan: "Love",
  },
  {
    gambar: "18.jpg",
    ucapan: "You",
  },
  {
    gambar: "19.jpg",
    ucapan: "Selamanya",
  },
  {
    gambar: "12.jpg",
    ucapan: "maaf untuk segala kesahalan aku",
  },
  {
    ucapan: "dadah"
  }
];

musik = "M1.mp3";
nomorWhatsapp = "6285885398458";

/*=========================*/
DekaTutorial(konten, musik, nomorWhatsapp);
</script></body></html>
