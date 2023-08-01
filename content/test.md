Title: 按鈕練習
Date: 2018-08-28 12:00
Category: Course
Tags: notes,steps,samples
Slug: 22_button1
Author: 40523122

<!-- PELICAN_END_SUMMARY -->

<!-- 導入 Brython 標準程式庫 -->
 
<script src="../data/Brython-3.3.1/brython.js"></script>
<script src="../data/Brython-3.3.1/brython_stdlib.js"></script>
 
<!-- 啟動 Brython -->
<script>
window.onload=function(){
// 設定 data/py 為共用程式路徑
brython({debug:1, pythonpath:['./../data/py']});
}
</script>

<script type="text/python3">

from browser import document, alert

def hello(ev):
    alert("Hello !")

document["button0"].bind("click", hello)




from browser import document

def change(event):
    document["zone1"].textContent = "New content"

document["button1"].bind("click", change)
def change(event):
        document["zone1"].text = "New Content"
</script>
<button id="button0">say hello</button>
<button id="button1">change</button>