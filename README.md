//How to copy URL on button click with javascript

<FRAME><div >
  <input type="button" value="Copy link" onclick="Copy();" style="font-family:IranYekan;font-size:14px;background-color:#ffffff;border-radius:32px;border:1px solid #ffffff;padding: 10px 15px 10px 15px;font-colore:#707070;" />
  <br /> <textarea id="url" rows="1" cols="30" 
    style="background-color:transparent;border-radius:32px;border:0px solid #707070;display: grid;font-colore:transparent;"></textarea>
</div>
</FRAME>
  <script>
 function Copy() {
  var Url = document.getElementById("url");
  Url.innerHTML = window.location.href;
  console.log(Url.innerHTML)
  Url.select();
  document.execCommand("copy");
}   
</script>
