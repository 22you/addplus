# addplus
实现购物车的加减
<pre><code>
<script>
function addPlus(e){
    var btn=e.getElementsByTagName('input');
    var stor=e.getElementsByTagName('strong')[0];
    var num=Number(stor.innerHTML);
     btn[0].onclick=function(){
      if(num>0){
        num--;
        stor.innerHTML=num;
      }
    }
    btn[1].onclick=function(){
      num++;
      stor.innerHTML=num;
    }
  }
  window.onload=function(){
   var regulation=document.getElementById('add-plus')
   addPlus(regulation)
  }
</script>
</code></pre>
## html代码


 
      <ul>
        <li>市场参考价格:<span>￥2000.00</span></li>
        <li>礼品编号：<span>SH001</span></li>
        <li>兑换时间：<span>无期限</span></li>
        <li>剩余数量：<span>998</span></li>
        <li>每个会员最多兑换：<span>无限制</span></li>
        <li>兑换数量：
            <div id="add-plus">
              <input type="button" class="addplus" value="-" />
              <strong>0</strong>
              <input type="button" class="addplus" value="+" />
            </div>
        </li>
      </ul>


