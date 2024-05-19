<!DOCTYPE html>
<html>
<head>
	<meta charset="utf-8">
	<meta name="viewport" content="width=device-width, initial-scale=1">
	<title>biy daalt 2</title>
</head>
<body>
	<h1 class="center">ТООЦООЛОЛ: НДШ-ийн 50%-ийн буцаан олголтоор та хэдэн
төгрөг авах боломжтой вэ?</h1>
	<p class="center">
		<span style="color:#FFFFFF;" >
			<span style="background-color:#2BE914;">&nbsp;ҮНДСЭН ЦАЛИН:
				&nbsp;
			</span>
		</span>
		&nbsp;
		<input placeholder="цалингаа оруулна уу" type="number" id="tsalin">
		<button class="button" onclick="tsaalin()">ЦАЛИН БОДОХ</button>
	</p>


	<table border="1" style="width:60%;" class="center">
	<thead>
		<tr class="ungu">
			<th>Агуулга</th>
			<th>
			<p>Одоо</p>
			<p>2022 (5-12 сар)</p>
			</th>
		</tr>
	</thead>
	<tbody>
		<tr>
			<td>
				ХХДХ<span>-Хөдөлмөрийн хөлсний доод хэмжээ</span>
			</td>
			<td id="1" class="saaral">
				
			</td>
		</tr>
		<tr>
			<td>
				НДШ (%)-Хувь хүн
			</td>
			<td id="2"class="saaral">
				
			</td>
		</tr>
		<tr>
			<td>
				НДШ (%)-АО
			</td>
			<td id="3"class="saaral">
				
			</td>
		</tr>
		<tr>
			<td>
				<div class="tsenher">ЦАЛИН БҮГД</div>
			</td>
			<td id="4" class="tsenher"></td>
		</tr>
		<tr>
			<td>
				НДШ-АО<span> - Ажил олгогчоос төлөх</span>
			</td>
			<td id="5" class="ulaan">
				
			</td>
		</tr>
		<tr>
			<td>
				<div class="nogoon">ҮНДСЭН ЦАЛИН<span>-Сарын үндсэн цалин</span></div>
			</td>
			<td id="6" class="nogoon">
				
			</td>
		</tr>
		<tr>
			<td>
				НДШ -Хувь хүн төлөх (2%+9.5%)
			</td>
			<td id="7" class="ulaan">
				
			</td>
		</tr>
		<tr>
			<td>
				ХХОАТ 10%
			</td>
			<td id="8" class="ulaan">
				
			</td>
		</tr>
		<tr>
			<td>
				Хөнгөлөлт<span> - ХХОАТ-ийн хөнгөлөлт</span>
			</td>
			<td id="9" class="nogooon">
				
			</td>
		</tr>
		<tr>
			<td>
				<div class="ulbar">ГАРТ ОЛГОХ</div>
			</td>
			<td id="10" class="ulbar">
				
			</td>
		</tr>
		<tr>
			<td>
				НДШ - Буцаалт (4.75%)
			</td>
			<td id="11" class="nogooon">
				
			</td>
		</tr>
	</tbody>
</table>
<p>
<div class="footer">Анхааруулга: Энэхүү тооцоолол нь таны цалингийн эцсийн үнэлгээ биш байж болохыг анхаарна уу.</div>
</p>

<style type="text/css">
	.ungu {
		background: #ACC9DB;
	}
	.center{
		margin-left: auto;
		margin-right: auto;
		text-align: center;
	}
	.button {
		height:32px;
		color: #fff;
		background: #054FF9;
		border-color: #054FF9;
		padding: 4px 6px;
		border-radius: 4px;
		margin-left: 4px;
	}
	.ulbar {
		 background: #F98405;
		 color: #fffff0;
	}
	.tsenher {
	 	background: #14B4E9;
	  	color: #fffff0
	}
	.nogoon {
	 	background: #2BE914;
	  	color: #fffff0;
	  	margin: 0;
	  	paddin: 0px;
	}
	.ulaan {
		color: #FA0808;
	}
	.nogooon {
		color: #08FA17;
	}
	.saaral {
		color: #CACFD2;
	}
	.footer{
		background-color: #CACFD2;
		width: 58%;
		margin-left: auto;
		margin-right: auto;
		text-align: center;
		height: 50px;
		border-radius: 10px;
		justify-content: center;
		align-items: center;
		display: flex;
	}
</style>
<script type="text/javascript">
	function tsaalin(){
		tsalin = document.getElementById("tsalin").value;
		bugd = parseInt(tsalin) * 112.5 / 100;
		ndsh = parseInt(tsalin) * 12.5 / 100;
		huvi = parseInt(tsalin) * 11.5 / 100;
		hhoat = parseInt(tsalin) * 8.85 /100;
		gar = parseInt(tsalin) * 88.5 / 100;
		butsaalt = parseInt(tsalin) * 4.75 / 100;
		document.getElementById("1").innerHTML = "(420.000)";
		document.getElementById("2").innerHTML = "(11.5%)";
		document.getElementById("3").innerHTML = "(12.5%)";
		document.getElementById("4").innerHTML = bugd;
		document.getElementById("5").innerHTML -= ndsh;
		document.getElementById("6").innerHTML = tsalin;
		document.getElementById("7").innerHTML -= huvi;
		document.getElementById("8").innerHTML -= hhoat;
		document.getElementById("9").innerHTML = "+" +hhoat;
		document.getElementById("10").innerHTML = gar;
		document.getElementById("11").innerHTML = butsaalt;
	}
</script>
</body>
</html>
