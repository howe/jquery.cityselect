# jquery.cityselect

######找了一大圈都没找到新的版本，所以自己整理一个了，数据源来源最新的2016年2月全国行政区域表，包含港澳台地区的行政区域。


* 用法

```javascript
<script src="https://cdn.bootcss.com/jquery/1.12.4/jquery.min.js"></script>
<script src="jquery.cityselect.min.js"></script>

jQuery(function () {
            jQuery("#city").citySelect({
				url:"jquery.cityselect.citylist.json",  //JSON数据源地址
				prov:"江苏", //省份
				city:"南京", //城市
				dist:"玄武区", //区县
				nodata:"none" //当子集无数据时，隐藏select
			});
        });


<div id="city">
    <select class="prov"></select>
    <select class="city" disabled="disabled"></select>
    <select class="dist" disabled="disabled"></select>
</div>
```