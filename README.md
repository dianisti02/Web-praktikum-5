# Web-praktikum-5
Dian Islamiati_0110120017_SI03
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
