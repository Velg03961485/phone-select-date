# phone-select-date
date select plug-in

这是一款使用手机端的h5 日期选择插件

通过引入样式和js 来实现

采用弹框，底部轮播选择日期

适配性好，使用方便

<link rel="stylesheet" href="mobileSelect.css" type="text/css"/>
<link rel="stylesheet" href="mobile-select-date.css" type="text/css"/>
	
<script type="text/javascript" src="dialog.js"></script>
<script type="text/javascript" src="mobile-select-date.js"></script>
	
	

<div class="textBox-phone" style="display: flex">
        <div class="phne-name">生日</div>
        <div class="userName" >
            <input type="text" placeholder="请选择您的生日" class="userInput" id="birthday" style="width: 4.1rem;font-size: 0.3rem;"/>
        </div>
</div>

js 创建新对象

var selectDate = new MobileSelectDate();

selectDate.init({
        trigger:'#birthday',min:'1700-01-01',max:null,position:"bottom"});
		
输出选择的元素
console.log($("#birthday").val().replace(/\//g, "-"))
