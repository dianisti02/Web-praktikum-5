# Web-praktikum-5
Dian Islamiati_0110120017_SI03
aplikasi chat & kalkulator kurs rupiah
<!DOCTYPE html>
<html>
    <head>
        <title>Chat</title>
    </head>
    <body>
        <div style="width:100%; stroke:black;" id="isi_chat">
            
        </div>
        <form methode="REQUEST" onsubmit="return kirim();">
        <input id="pesan" style="width: 50%" type:"text" name="pesan">
        <button type="submit" onclick="return kirim();">KIRIM PESAN</button>
            
        </form>
    </body>
    <script type="text/javascript">
    function kirim(){
        let pesan= document.getElementById("pesan").value;
        document.getElementById("isi_chat").innerHTML += pesan+"<br/>";
        document.getElementById("pesan").value = "";
        return false;
    }
    
    </script>
    
</html>


<!DOCTYPE html>
<html>
    <head>    
        <title>Kurs Rupiah</title>
    </head>
    <body>    
    
    <center>        
    <table border="1" style="width: 30%">            <tr>                
    <td>Masukan Nilai</td>          
    <td>Value</td>                
    <td>Nilai Rupiah</td>            
    </tr>            
<tr>
    <td>
        <input onkeyup="kurs()" style="width: 90%" placeholder="Masukan Nilai" type="text" name="nilai" id="nilai">
    </td>
    <td>
        <select onchange="kurs()" id="kurs" style="width: 90%">
            <option value="0">Ubah Kurs</option>                    
            <option value="1">Dollar US</option>                    
            <option value="2">Dollar Singapore</option>                    
            <option value="3">Ringgit Malaysia</option>                    
            <option value="4">Yen Jepang</option>                    
            <option value="5">Euro</option>
                
            <option value="6">Riyal Arab Saudi</option>                
         </select>
    </td>                
    <td>
        <input type="text" disabled="" id="rupiah" placeholder="Nilai Rupiah" style="width: 90%" name="rupiah">
    </td>            
    </tr>        
    </table>    
    </center>
        
    </body>
        
    <script type="text/javascript">    
    function kurs() {         
    let k=
    document.getElementById("kurs").value;
    if (k == 1) {            
    input =
    document.getElementById("nilai").value;
    nilai = 9915;            
    hitung = nilai * input;
    document.getElementById("rupiah").value =
    hitung;}
    else if (k == 2) {            
    input =
    document.getElementById("nilai").value;
    nilai = 13472;            
    hitung = nilai * input;
    document.getElementById("rupiah").value =
    hitung;}
    else if (k == 3) {            
    input =
    document.getElementById("nilai").value;
    nilai = 874;            
    hitung = nilai * input;
    document.getElementById("rupiah").value =
    hitung;}
    else if (k == 4) {            
    input =
    document.getElementById("nilai").value;
    nilai = 120;            
    hitung = nilai * input;            
    document.getElementById("rupiah").value =
    hitung;}
    else if (k == 5) {            
    input =
    document.getElementById("nilai").value;
    nilai = 15888;            
    hitung = nilai * input;
    document.getElementById("rupiah").value =
    hitung;}
    else if (k == 6) {            
    input =
    document.getElementById("nilai").value;
    nilai = 3592;            
    hitung = nilai * input;
    document.getElementById("rupiah").value =
    hitung;} }
    </script>
        
    </html>
