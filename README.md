//How to copy URL on button click with javascript

<FRAME><div >
  <input type="button" value="کپی لینک" onclick="CopyUrl(); HideUrl();" style="font-family:IranYekan;font-size:14px;background-color:#ffffff;border-radius:32px;border:1px solid #ffffff;padding: 10px 15px 10px 15px;font-colore:#707070;" />
  <br /> <textarea id="url" rows="1" cols="30" style="display:none"></textarea>
</div>
</FRAME>
  <script>
  function CopyUrl() {
    const url = window.location.href;
    navigator.clipboard.writeText(url);
    alert("URL copied to clipboard!");
  }
  
  function HideUrl() {
    document.getElementById("url").style.display = "none";
  }
</script>```

The `navigator.clipboard.writeText()` method is used to write text to the clipboard. The `url` parameter is used to specify the text that is being copied.

I hope this code works for you.

