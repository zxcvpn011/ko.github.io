<!DOCTYPE html PUBLIC -//W3C//DTD XHTML 1.0 Strict//EN http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd>
 <html lang="en">
 <head>
	 <title></title>
	 <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
	 <meta name="viewport" content="initial-scale=1.0">
	 <link rel="stylesheet" href="" type="text/css"/>
	  <link rel="stylesheet" href="https://use.fontawesome.com/releases/v5.3.1/css/all.css" />
	 <script src="jquery-3.4.1-new.js"></script>
	 <style>
	 		body { 
	 				padding: 0;
	 				margin:0;
	 				font-family: sans-serif;
	 		}
	 		button , input , textarea { 
	 				border:0;
	 				outline:0;
	 		}
	 		a { 
	 				text-decoration: none;
	 				-webkit-tap-highlight-color: transparent;
	 		}
	 		
/*						Navigation Bar Style				*/
	 		
	 		nav { 
	 				background: #000;
	 				color: #fff;
	 				padding: 20px;
	 				position: relative;
	 				/*animation: fade 1s;
			animation-fill-mode: forwards;
			animation-iteration-count: 1*/
	 		}
	 		.logo { 
	 				font-size: 25px;
	 				margin-left: -5px;
	 		}
	 		.logoColor { 
	 				color: #03fab3
	 		}
	 		.bars { 
	 				position: absolute;
	 				top: 20px;
	 				right: 15px;
	 				font-size: 30px;
	 		}
	 		.fa-times { 
	 				animation: 0.5s spin;
	 		}
	 		@keyframes spin { 
	 				from { 
	 						transform: rotate(0)
	 				}
	 				to {
	 						transform: rotate(-360deg)
	 				}
	 		}
	 		#menu { 
	 				margin-top: 30px;
	 				margin-right: -5px ;
	 				margin-left:-5px;			
	 				text-align: center;
	 				overflow: auto;
	 				height: 250px;
	 				
	 				/*position: fixed;
	 				background: #000;
	 				top: -20px;
	 				bottom: 0;
	 				color: #fff;
	 				z-index: 99;*/
	 		}
	 		.caption { 
	 				text-align: center;
	 				font-size: 35px;
	 				width: 70%;
	 				margin: auto;
	 				padding: 20px;
	 				border-bottom: 2px solid #000;
	 				margin-bottom: 45px;
	 		}
	 		.menuOptions { 
	 				color: #fff;
	 				display: block;
	 				text-align: center;
	 				padding: 25px;
	 				margin-top: 5px;
	 				background: rgb(0, 102, 185);
	 				transition: 0.3s;
	 		}
	 		.menuOptions:last-child { 
	 				margin-bottom: 30px;
	 		}
	 		.menuOptions:hover { 
	 				background: rgb(86, 0, 176);
	 				color: #fff;
	 		}
	 		.menuOptions > .fas { 
	 				font-size: 18px;
	 		}
	 		.menuOptions > .fab { 
	 				font-size: 18px;
	 		}
	 		
/*				jQuery Animation onscroll		*/

	 		@keyframes fade { 
	 				from { 
	 						opacity:0;
	 				}
	 				to {
	 						opacity:1;
	 				}
	 		}
	 		@keyframes fade2 { 
	 				from { 
	 						padding-bottom: 20px;
	 				}
	 				to {
	 						padding-bottom: 28px;
	 				}
	 		}
	 			 		
	/*							Header Style						*/
	 		
	 		header { 
	 				display: flex;
	 				align-items: center;
	 				justify-content: center;
	 				height: 300px;
	 				background: lightyellow;
	 				color: #fff;
	 				flex-direction: column;
	 		}
	 		header > .cap { 
	 				white-space: pre-wrap;
	 				text-align: center;
	 				font-size: 30px;
	 				padding: 50px 20px 40px 20px ;
	 				margin:0;
	 				color: #000;
	 		}
	 		.hedBtn { 
	 				color: #fff;
	 				display: block;
	 				text-align: center;
	 				padding: 25px;
	 				margin-top: 5px;
	 				background: rgb(0, 102, 185);
	 				transition: 0.3s;
	 				
	 		}
	 		
	 		.hedBtn:last-child { 
	 				margin-bottom: 50px;
	 		}
	 		.hedBtn:hover { 
	 				background: rgb(86, 0, 176);
	 				color: #fff;
	 		}	
	 		
/*						+ Code & Result Sec				*/

	 		section { 
	 				margin-bottom: 25px;
	 				margin-top: 10px;
	 		}
	 		.description { 
	 				padding: 20px;
	 				text-align: center;
	 		}
	 		.deskCap { 
	 				border-bottom: 1px solid #ppp;
	 				display: table;
	 				margin: auto;
	 				padding-bottom: 10px;
	 		}
	 		.description , #result { 
	 				word-break: break-word;
	 		}
	 		b { 
	 				padding: 20px;
	 				text-align: center;
	 				display: block;
	 		}
	 		.bold { 
	 				font-weight: bold;
	 		}
	 		#txt { 
	 				height: 200px;
	 				width: 80%;
	 				margin: auto;
	 				display: block;
	 				border: 2px solid #000;
	 				font-size: large;
	 				white-space: pre-wrap;
	 		}
	 		#submit , .btn{ 
	 				width: 150px;
	 				padding: 15px;
	 				text-align: center;
	 				background: dodgerblue;
	 				margin: auto;
	 				color: #fff;
	 				margin-top: 25px;
	 		}
	 		#submit:hover , .btn:hover { 
	 				background: red;
	 		}
	 		
	 		#result { 
	 				padding: 20px;
	 				white-space: pre-wrap;
	 		}
	 		.copyBtn { 
	 				padding: 20px;
	 				text-align: center;
	 				background: #000;
	 				color: #fff;
	 				width: 70%;
	 				margin: 10px auto;
	 				transition: 0.3s;
	 		}
	 		.copyBtn:hover { 
	 				background: #0066ff;
	 		}
	 		
	/*				HTML DOC Opt Style				*/
	
	 		.plusBtn { 
	 				text-decoration: underline;
	 				margin: 20px;
	 				margin-top: 55px;
	 				font-size: 20px;
	 		}
	 		#getSelectOptCon {
	 				text-align: center;
	 				margin-bottom: 25px;
	 				display: none;	
	 		}
	 		.replaceCon {
	 				margin-bottom: 15px;
	 		}
	 		.replaceCon > .caption {
	 				border:0;
	 				padding:0;
	 				font-size: 30px;
	 				margin-top: 60px;
	 		}
	 		.replaceDescription { 
	 				margin-bottom: 15px;
	 				padding: 10px;
	 		}
	 		.replaceTxtField {
	 				padding:15px;
	 				border-bottom: 2px solid #000;
	 				font-size: medium;
	 				width: 60%;
	 				display: inline-block;
	 		}
	 		.replaceBtn {
	 				padding: 15px;
	 				background: #0066ff;
	 				color:#fff;
	 				display: inline-table;
	 		}
	 		.replaceBtn:hover {
	 				background: #1c1d22;
	 		}
	 		.optContainer { 
	 			display: none;
	 		}
	 		.getSelectOpt {
	 				background: #181818;
	 				padding: 20px;
	 				color: #fff;
	 				margin: 1px auto;
	 				transition: 0.3s;
	 				width: 75%;
	 		}
	 		.getSelectOpt4, .getSelectOpt5 {
	 				background: #333;
	 		}
	 		.getSelectOpt3 { 
	 				background: #0066ff;
	 				color: #fff;
	 		}
	 		.getSelectOpt:hover {
	 				background: red;
	 		}
	 		.moreOpt { 
	 				padding: 15px;
	 				text-align: center;
	 				background: dodgerblue;
	 				color: #fff;
	 				margin-top: 5px;
	 				display: inline-table;
	 		}
	 		.moreOpt:nth-child(3) { 
	 				background: #000;
	 		}
	 		.moreOpt:nth-child(4) { 
	 				background: red;
	 		}
	 		.moreOpt:nth-child(5) { 
	 				background: #fff;
	 				box-shadow: 2px 1px 2px 1px rgba(0,0,0,0.2);
	 				color: #000;
	 		}
	 		.moreOpt:nth-child(7) { 
	 				background: #0066ff;
	 				box-shadow: 2px 1px 2px 1px rgba(0,0,0,0.2);
	 				color: #fff;
	 		}
	 		.moreOpt:nth-child(9) { 
	 				background: red;
	 				box-shadow: 2px 1px 2px 1px rgba(0,0,0,0.2);
	 				color: #ffff;
	 		}
	 		.moreOptCon { 
	 				text-align: center;
	 				padding-top: 15px;
	 				display: none;
	 		}
	 		.moreOptCon > .caption { 
	 				border-color: transparent;
	 				margin-bottom: 5px;
	 				font-size: 30px;
	 		}
	 		.moreOpt:hover { 
	 				background: #e91e63;
	 				color: #fff;
	 		}
	 		
/*					EcmaScript Opt Style					*/
	 		
	 		.jsOpt { 
	 				display: none;
	 		}
	 		.jsOpt , .jsOptBtn { 
	 				width: 80%;
	 				margin: auto;
	 				padding: 20px;
	 				text-align: center;
	 				color: #fff;
	 				background: #000;
	 		}
	 		.jsOpt > .caption { 
	 				border:0
	 		}
	 		.jsOptBtn { 
	 				background: red;
	 				margin-top: 25px;
	 				margin-bottom: 25px;
	 				padding: 15px
	 				
	 		}
	 		.jsOptBtn:hover { 
	 				background: rgb(16, 175, 60);
	 				color: #fff;
	 		}
	 		.exTxt { 
	 				padding: 15px;
	 				text-align: center;
	 		}
	 		
/*							Footer Section								*/

	 		footer { 
	 				background: #000;
	 				padding: 25px;
	 				text-align: center;
	 				overflow: hidden;
	 		}
	 		footer > :nth-child(1) { 
	 				display: table;
	 				margin: auto;
	 				font-size: 22px;
	 				color: #fff;
	 		}
	 </style>
 </head>
	 <body>

<!--			Navigation Bar Section				-->

		<nav>
			<div class="logo">
				Programmer<span class="logoColor">Helper</span>
			</div>
			<div class="bars">
				<i class="fas fa-bars"></i>
			</div>
			
			<div id="menu">
			<div class="caption">HTML</div>
				<a href="#codeSec"  class="menuOptions getSelectors">Get classs + Id 
					<i  class="fas fa-arrow-right"></i>
					<i  class="fas fa-file-code"></i>
				</a>
				<div class="caption">CSS</div>
				<a href="#codeSec"  class="menuOptions addVK">
				add Vendor Prefix 
				<i  class="fas fa-arrow-right"></i>
				@</a>
				<a href="#codeSec"  class="menuOptions addV">
				add Vendor Prefix 
				<i  class="fas fa-arrow-right"></i>
				Props</a>
				<a href="#codeSec"  class="menuOptions cssCurly">
				add
				 { } 
				<i  class="fas fa-arrow-right"></i>
				 CSS Selectors</a>
				<a href="#codeSec"  class="menuOptions cssDot">
				add
				 .dot 
				<i  class="fas fa-arrow-right"></i>
				 classes</a>
				<a href="#codeSec"  class="menuOptions cssHash">
				add
				 #hash 
				<i  class="fas fa-arrow-right"></i>
				 id's</a>
				 <a href="#codeSec"  class="menuOptions cssSelectorsOnly">
				get selectors only 
				<i  class="fas fa-arrow-right"></i>
				CSS
				<i  class="fas fa-file"></i>
				 </a>
				  <a href="#codeSec"  class="menuOptions cssPropsOnly">
				get properties only 
				<i  class="fas fa-arrow-right"></i>
				CSS
				<i  class="fas fa-file"></i>
				 </a>
				 <div class="caption">jQuery</div>
				 <a href="#codeSec"  class="menuOptions jqTag">Tags Name 
				<i  class="fas fa-arrow-right"></i>
				 $</a>
				<a href="#codeSec"  class="menuOptions jqClass">classes 
				<i  class="fas fa-arrow-right"></i>
				 $</a>
				<a href="#codeSec"  class="menuOptions jqId"> id's 
				<i  class="fas fa-arrow-right"></i>
				 $</a>
				 <a href="#codeSec"  class="menuOptions jqMultiSelect"> all selectors: # , dot , tag 
				<i  class="fas fa-arrow-right"></i>
				 $</a>
				 <div class="caption">JavaScript</div>
				 <a href="#codeSec"  class="menuOptions jsTag">Tags Name 
					<i  class="fas fa-arrow-right"></i>
					<i  class="fab fa-js"></i>
					</a>
					<a href="#codeSec"  class="menuOptions jsClass">classes 
					<i  class="fas fa-arrow-right"></i>
					<i  class="fab fa-js"></i>
					</a>
				<a href="#codeSec"  class="menuOptions jsId"> id's
				<i  class="fas fa-arrow-right"></i>
					<i  class="fab fa-js"></i>
				</a>
				<div class="caption">Creating Elements</div>
					<a href="#codeSec"  class="menuOptions jsConvert">Convert 
					<i  class="fas fa-code"></i>
					<i  class="fas fa-arrow-right"></i>
					<i  class="fab fa-js"></i>
					 </a>
					 <a href="#codeSec"  class="menuOptions jqConvert">Convert 
				<i  class="fas fa-code"></i>
				<i  class="fas fa-arrow-right"></i>
				 jQuery
				 </a>
					
			</div>
		</nav>
		
<!--						Header Section						-->
		
		<header>
<div class="cap">Click ON Navigation Bar To Find Your Options</div>
<!--
Choose Your Option
<div class="hedBtn">Check Navigation Options</div>
<div class="hedBtn">Create Special RegExp</div>
-->
		</header>
		
<!--						Textarea Section					-->
		
		<section id="codeSec">
			<div class="caption">Code Section</div>
			<div>
				<b class="deskCap">Description</b>
				<div class="description">
				Undefined
				</div>
			</div>
			<b>
			<i  class="fas fa-plus"></i>
			 Your Code</b>
			 <textarea id="txt"></textarea>
			 <div id="submit" class="sub">Submit</div>
		</section>
		
<!--							Results Section					-->
		
		<section>
			<div class="caption">Result</div>
			<div id="result">
			<b>You Will See Your Result And Options Here</b>
			</div>
			<div class="htCopyBtn copyBtn">Copy Your Code</div>
			
	<!--						HTML DOC Options			-->
			
			<div id="getSelectOptCon">
			<div class="replaceCon">
			<div class="caption">Replace Section</div>
			<div class="replaceDescription">if The Result have repeated words - write the repeated word in this field to remove all repeated word and keep only one</div>
			<input type="text"  class="replaceTxtField" placeholder="write repeated word here...">
			<button class="replaceBtn">Replace</button>
			</div>
			<div class="plusBtn showMore">
			<i class="fas fa-plus"></i>
			More Options</div>
			<div class="optContainer">
			<div class="getSelectOpt getSelectOpt1">
					Remove all selectors with dot
				</div>
				<div class="getSelectOpt getSelectOpt2">
					Remove all selectors with #
				</div>
				<div class="getSelectOpt getSelectOpt3">
					Remove # , dot
				</div>
				<div class="getSelectOpt getSelectOpt4">
					Remove # only
				</div>
				<div class="getSelectOpt getSelectOpt5">
					Remove dot only
				</div>
			
		
			<div class="caption">CSS Options</div>
			<!--<div class="moreOpt">
				<i  class="fas fa-plus"></i>
				.dot
			</div>
			<div class="moreOpt">
			<i  class="fas fa-plus"></i>
				#hash
			</div> -->
			<div class="moreOpt">
			<i  class="fas fa-plus"></i>
				curly brackets
			</div>
			<div class="caption">jQuery Options</div>
			<div class="moreOpt">
				create selector
			</div>
			<div class="moreOpt">
				<i  class="fas fa-plus"></i>
				click , function
			</div>
			<div class="caption">JS Options</div>
			<div class="moreOpt">
				<div>Convert</div> 
					#id 
					<i class="fas fa-arrow-right"></i> JS 
			</div>
			<div class="moreOpt">
				<div>Convert</div> 
					.classes 
					<i class="fas fa-arrow-right"></i> JS 
			</div>
			<div class="moreOpt">
				<i  class="fas fa-plus"></i>
				EventListemer , function
			</div>
			</div>
			</div>
<!--					JavaScript Options				-->
			
			<div class="jsOpt">
			<div class="caption">JS Options</div>
				<div class="jsOptBtn xIndex">Remove Index</div>
				<div class="jsOptBtn xSemi">Remove Semi Colon</div>
				<div class="noteTxt">
					<i class="bold">Attention</i>
					<div class="noteWords">Be careful when using the following option because maybe one of your selectors name looks like js reversed word - look at js reversed word before using this Button - or you can use it directly but be careful</div>
				</div>
				<div class="jsOptBtn DeclareBtn">Declare Variables With The Same Selector Name</div>
			</div>
			
			<!--	<div class="jsOptBtn">remove space quote</div> -->
			</div>
		</section>
		
<!--									Footer Sec							-->
		
		<footer>
			<div>©Programmer<span class="logoColor">Hepler.com</span></div>
		</footer>
		<script>
		
/*									Styling Page								*/


$("#menu").hide();
$(".bars").click(function() {
	$("#menu").slideToggle();

	$(".bars > :nth-child(1)").toggleClass("fa-times");
});

$( ".menuOptions").click(function() { 
		$("#codeSec").slideDown();
		$("#menu").hide(200);
		$(".bars > :nth-child(1)").attr("class", "fas fa-bars");
});

$("a").click(function(e) {
		e.preventDefault();
    var a = $("a").attr("href");
    $('html,body').animate({scrollTop: $(a).position().top}, 800, "linear");
});


$(window).scroll(function(e) { 
	if( $(window).scrollTop() > $("nav").height() ) {

		$("nav").css({
			position:  "fixed",
			right: 0,
			left:0,
			background: "#000",
			top:0,
			"animation": "1s fade",
		});
		
	} 
		if ($(window).scrollTop() < 2 ) { 
		$("nav").css("animation", "0.5s fade2");
		$("nav").css({
			position:  "relative",
			"animation": "fade2 0.4s",
			"animation-fill-mode": "forwards"
		});
	}
}); 
$(".showMore").click(function() { 
	$(".optContainer").slideToggle("slow");
});

$(".copyBtn").click(function() { 
	/*var CopyElem = "<textarea id='CopyElem' style='white-space:pre-wrap'></textarea>";
	$("body").append(CopyElem);
	if($("#CopyElem").val() == "") {
		$("#CopyElem").val($("#result").text());
	}
	$("#CopyElem").select();
	document.execCommand("copy");
	var removeElem = $("#CopyElem").remove();
	setTimeout(removeElem,0);*/
	
	var Txt_A = res.innerText;
	var Elem_A = document.createElement("textarea");
	Elem_A.setAttribute("class" , "Elem_A");
	Elem_A.setAttribute("style" , "white-space: pre-wrap;");
	document.body.appendChild(Elem_A);
	var TxtCon_A = document.getElementsByClassName("Elem_A")[0];

	if (TxtCon_A.value == "") {
		TxtCon_A.value = Txt_A;
	}

	TxtCon_A.select();
	document.execCommand("copy");

	var XTag_A = $(".Elem_A").remove();
	setTimeout(XTag_A, 0);
	
			
});


	/*					Programmer Options					*/


//							Main Elements

var res = document.getElementById("result");
var txt = document.getElementById("txt");
var sub = document.getElementById("submit");
var desk = document.getElementsByClassName("description")[0];


//								Menu Options Btn

var getSelectors = document.getElementsByClassName("getSelectors")[0];
var cssCurly = document.getElementsByClassName("cssCurly")[0];
var cssDot = document.getElementsByClassName("cssDot")[0];
var cssHash = document.getElementsByClassName("cssHash")[0];
var cssSelectorsOnly = document.getElementsByClassName("cssSelectorsOnly")[0];
var cssPropsOnly = document.getElementsByClassName("cssPropsOnly")[0];
var jqTag = document.getElementsByClassName("jqTag")[0];
var jqClass = document.getElementsByClassName("jqClass")[0];
var jqId = document.getElementsByClassName("jqId")[0];
var jqMultiSelect = 
document.getElementsByClassName("jqId")[0];
var jqMultiSelect = document.getElementsByClassName("jqMultiSelect")[0];
var jsTag = document.getElementsByClassName("jsTag")[0];
var jsClass = document.getElementsByClassName("jsClass")[0];
var jsId = document.getElementsByClassName("jsId")[0];
var jsConvert = document.getElementsByClassName("jsConvert")[0];
var jqConvert = document.getElementsByClassName("jqConvert")[0];
var addVK = document.getElementsByClassName("addVK")[0];
var addV = document.getElementsByClassName("addV")[0];


//									Choices

var choice1 = document.getElementById("getSelectOptCon");

//Logo

var logo = document.getElementsByClassName("logo")[0];

//The Following RegEx To remove The Empty line what who made when the user write new empty lines or add id or class inside JS , JQ  tags function

var removeEmptyLines = new RegExp("\n" + "", "ig");
		


/*								 HTML options 							*/

//	>>>>>>>>>>>> Btn1 <<<<<<<<<<<<

getSelectors.addEventListener('click' , function() { 
	
	sub.className = "selectorsBtn";
	var selectorsBtn =	document.getElementsByClassName("selectorsBtn")[0];
	
	var deskStr1 = "This option allows you to get all selectors from HTML document to use it in " + "<i class='bold'>CSS ,  jQuery</i>";
	
	desk.innerHTML = deskStr1;
		
		selectorsBtn.addEventListener("click", function(event) { 
		
		res.innerHTML = txt.value.match(/(id=".*?")|(class=".*?")/igm)
		res.innerHTML = res.innerHTML.replace(/id=/g, "#").replace(/class=/g, ".").replace(/"/g,"").replace(/,/g, "<br />").replace(/\s/g , "\n.");
		
		 if(this.className == "selectorsBtn") {
	 	choice1.style.display = "block";
	 } else {
	 		choice1.style.display = "none";
	 }
		
	});
		

});


/*								CSS options									*/

//	>>>>>>>>>>> #Btn1 <<<<<<<<<<<<



addVK.addEventListener("click",function() { 
		sub.className = "addVKBtn";
	logo.innerHTML = sub.className;
	var addVKBtn = document.getElementsByClassName("addVKBtn")[0];
	
	addVKBtn.addEventListener("click",function() { 
		var matchPro = txt.value.match(/(\w|\W).*?/g);
		var Vendor1K = "";
		var Vendor2K = "";
		var Vendor3K = "";
		var Vendor4K = "";
		
		for(var k = 0; k < matchPro.length; k++) { 
		Vendor1K += matchPro[k].replace(/@/g, "@-webkit-") ;
		Vendor2K += matchPro[k].replace(/@/g, "\n@-ms-")
	Vendor3K += 	matchPro[k].replace(/@/g, "\n@-o-");
		Vendor4K += matchPro[k].replace(/@/g, "\n@-moz-");
		}
		res.innerText = Vendor1K + Vendor2K + Vendor3K + Vendor4K
	});
	
});



addV.addEventListener("click",function() { 
		sub.className = "addVBtn";
	logo.innerHTML = sub.className;
	var addVBtn = document.getElementsByClassName("addVBtn")[0];
	
	addVBtn.addEventListener("click",function() { 
		var matchProP = txt.value.match(/(\w|\W).*/g);
		var Vendor1P = "";
		var Vendor2P = "";
		var Vendor3P = "";
		var Vendor4P = "";
		
		for(var p = 0; p < matchProP.length; p++) { 
		Vendor1P += matchProP[p].replace(/a.*?n\b/ig, "-webkit-animation")
		Vendor2P += matchProP[p].replace(/animation/ig, "-ms-animation").replace(/transition/ig, "-ms-transition")
	Vendor3P += 	matchProP[p].replace(/animation/ig, "-o-animation").replace(/transition/ig, "-o-transition")
		Vendor4P += matchProP[p].replace(/animation/ig, "-moz-animation").replace(/transition/ig, "-moz-transition")
		}
		res.innerText = Vendor1P + "\n" + Vendor2P + "\n" + Vendor3P + "\n" + Vendor4P
	});
	
});


cssCurly.addEventListener('click' , function() { 
	
	sub.className = "addCurlyBtn"
	var addCurlyBtn =	document.getElementsByClassName("addCurlyBtn")[0];
	
	desk.innerHTML = "This option allows you to add curly brackets to css selectors like id , class , tagNames " + "<div style='padding: 30px;'><i class='bold'>#Note:</i>" + " The css selectors should to be followed by new line like the following example</div>" + "<ul style='text-align:left'>" + 
	"<li>body</li>" + 
	"<li>div</li>" + 
	"<li>#container</li>" + 
	"<li>#header</li>" +
	"<li>.text</li>" + 
	"<li>.link</li>" + 
	"<li>etc...</li>" +
	"</ul>";
	
	
	addCurlyBtn.addEventListener("click", function() { 
		/*res.innerHTML = txt.value.replace(/\n\./g," {\n\t\t\n}\n") +  " ";
		res.innerHTML = txt.value.replace(/#/g," {\n\t\t\n}\n") +  " ";
		res.innerHTML = res.innerHTML.replace(/(.)$/g, " {\n\t\t\n}");*/
		
		var myArr = [];
	var myloop = "";
	txt.value = "\n" + txt.value;
	var x = txt.value.match(/\n.*/g);
	for (var tt = 0; tt < x.length; tt ++) { 
	 myArr.push(x[tt]);
	 myloop += '<div class="curlyLoopClass">' +  myArr[tt] + '</div>';
	}
	var appendElem = document.createElement("div");
	appendElem.setAttribute("style", "display:none")
	appendElem.setAttribute("id", "ElemId");
	document.body.appendChild(appendElem);
	var y = document.getElementById("ElemId");
	y.innerHTML = myloop;
	
	var CurlyVar = document.getElementsByClassName("curlyLoopClass");
	var newloop = "";
	
	for ( var qq = 0; qq < CurlyVar.length; qq++) { 
		newloop += "<div>" + CurlyVar[qq].innerHTML + " {\n\t\t\n}" + "</div>";
	}
		res.innerHTML =  newloop;
	
	});

});

//	>>>>>>>>>>> #Btn2 <<<<<<<<<<<<

cssDot.addEventListener('click' , function() { 
	
	sub.className = "addDotCSSBtn";
	var addDotCSSBtn =	document.getElementsByClassName("addDotCSSBtn")[0];
	
	desk.innerHTML = "This option allows you to add dot for your class names " + "<div style='padding: 30px;'><i class='bold'>#Note:</i>" + " class names should to followed by new line like the following example</div>" + "<ul style='text-align:left'>" + 
	"<li>class1</li>" + 
	"<li>class2</li>" + 
	"<li>class3</li>" + 
	"<li>...</li>" +
	"</ul>";
		
	
	
	addDotCSSBtn.addEventListener("click", function() { 
		
		res.innerHTML =  "." + txt.value.replace(/\s*[^\w.*?]/ig, "?").replace(/\?/g, "\n.").replace(/(\n\.)$/g , "");;
		
	
	});

});


//	>>>>>>>>>>> #Btn3 <<<<<<<<<<<<


cssHash.addEventListener('click' , function() { 
	
	sub.className = "addHashCSSBtn";
	var addHashCSSBtn =	document.getElementsByClassName("addHashCSSBtn")[0];
	
	desk.innerHTML = "This option allows you to add #hash for your id's " + "<div style='padding: 30px;'><i class='bold'>#Note:</i>" + " id should to followed by new line like the following example" + "</div>" + "<ul style='margin-top: 0px;text-align:left'>" + 
	"<li>id1</li>" + 
	"<li>id2</li>" + 
	"<li>id3</li>" + 
	"<li>...</li>" +
	"</ul>";
		
	
	
	addHashCSSBtn.addEventListener("click", function() { 
		
		res.innerHTML =  "#" + txt.value.replace(/\s*[^\w.*?]/ig, "?").replace(/\?/g, "\n#").replace(/(\n#)$/g , "");;
		
	});

});


//	>>>>>>>>>>> #Btn4 <<<<<<<<<<<<


cssSelectorsOnly.addEventListener('click' , function() { 
	
	sub.className = "getCSSselectors";
	var getCSSselectors =	document.getElementsByClassName("getCSSselectors")[0];
	
	desk.innerHTML = "This option allows you to get all selectors from CSS stylesheet like id , class , tagName , pseudo selectors , etc... ";
	
	
	getCSSselectors.addEventListener("click", function() { 
	
	res.innerHTML = txt.value.replace(/{([^}]+)}/g , "").replace(/\t/g, "").replace(/\s\t/g, "").replace(/\n/g , "£").replace(/\t\s/g, "").replace(/£/g, "\n").replace(/\}/g , "").replace(/\{/g , "");
		
	});

});


//	>>>>>>>>>>> #Btn5 <<<<<<<<<<<<



cssPropsOnly.addEventListener('click' , function() { 
	
	sub.className = "getCSSproperties";
	var getCSSproperties =	document.getElementsByClassName("getCSSproperties")[0];
	
	desk.innerHTML = "This option allows you to get all CSS Properties from CSS stylesheet like ";
		
	
	
	getCSSproperties.addEventListener("click", function() { 
	
	res.innerHTML = txt.value.match(/{([^}]+)}/g );
	res.innerHTML = res.innerHTML.replace(/\t/g, "").replace(/\s\t/g, "").replace(/\n/g , "£").replace(/\t\s/g, "").replace(/£/g, "\n").replace(/\}/g , "").replace(/\{/g , "").replace(/,/g , "");
		
	});
});

/*								jQuery options								*/

//	>>>>>>>>>>> $Btn1 <<<<<<<<<<<<


jqTag.addEventListener("click", function() { 
	sub.className = "jQueryTagName";
	
	desk.innerHTML =  'This option allows you to put selectors inside $("selector") - this option can save many time for you to declare selectors inside variables and use them like you want in your jQuery Code ' + "<div style='padding: 30px'><i class='bold'>#Note</i></div>" + "your selectors should to be separated by new line like the following Example" + "<ul style='margin-top: 10px;text-align:left'>" + 
	"<li>selector1</li>" + 
	"<li>selector2</li>" + 
	"<li>selector3</li>" + 
	"<li>etc...</li>" +
	"</ul>";
	var JQTag = document.getElementsByClassName("jQueryTagName")[0];
	
	JQTag.addEventListener("click", function() { 
	
	/*
	//This an Element To Get the value of text box inside him to hide replaced words for user 
	
	var SelectorsConElem = document.createElement("div");
	SelectorsConElem.setAttribute("style" , "white-space: pre-wrap;display: none")
	
SelectorsConElem.setAttribute("id" , "TagSelectorsCon");

document.body.appendChild(SelectorsConElem);

var TagSelectorsCon = document.getelementById("TagSelectorsCon");

TagSelectorsCon.innerHTML = "£" + txt.value.replace(/\t/g, "").replace(/\s\t/g, "").replace(/\n/g , "£").replace(/\t\s/g, "").replace(/\n/g, "£").replace(/{/g , " {\n").replace(/}/g , "}\n").replace(/;/g , ";\n").replace(/£{1,100}/g, "£");;

	*/
	
	//This replace To replace all newLines made by user with any character To Keep Only one - but not working good yet 
	
	txt.value = txt.value.replace(/\t/g, "").replace(/\s\t/g, "").replace(/\n/g , "£").replace(/\t\s/g, "").replace(/\n/g, "£").replace(/£{1,100}/g, "£");;
	txt.value = "\n" + txt.value;
	
		var arr_A = []; // an array to collect the strings that are found
	var RegExp_A = /£(\w*)/g; // To Select All Text Between Curly Braces
	var str_A = txt.value;
	var collectStr_A;
	var loopRes= "";
	
//		Loop To Loop Text Between {} inside an array
	
	while (collectStr_A = RegExp_A.exec(str_A)) { 
		arr_A.push(collectStr_A[1]);
	}
	
//			Display Array Content

		
		for ( var i = 0 ; i < arr_A.length; i++) { 
				loopRes += "<div>" + "€" + arr_A[i] + "¥" + "</div>"
		}
		
		res.innerHTML = loopRes;
		res.innerHTML = res.innerText.replace(/€/g , '$("').replace(/¥/g , '");').replace(/\$\(\"\"\);/g, "").replace(removeEmptyLines, "").replace(/;/g, ";\n");
	});
	
});


//	>>>>>>>>>>> $Btn2 <<<<<<<<<<<<

jqClass.addEventListener("click", function () { 
	sub.className = "myJQClass";
	
	desk.innerHTML =  'This option allows you to put selectors inside $("selector") - this option can save many time for you to declare selectors inside variables and use them like you want in your jQuery Code ' + "<div style='padding: 30px'><i class='bold'>#Note</i></div>" + "your selectors should to be separated by dot and new line like the following Example" + "<ul style='margin-top: 10px;text-align:left'>" + 
	"<li>.selector1</li>" + 
	"<li>.selector2</li>" + 
	"<li>.selector3</li>" + 
	"<li>.etc__</li>" +
	"</ul>";
	
	var myJQClass = document.getElementsByClassName("myJQClass")[0];
	
	myJQClass.addEventListener("click", function() { 
		var txt = document.getElementById("txt");
		var arr_C = []; // an array to collect the strings that are found
	var RegExp_C = /\.(\w*)/g; // To Select All Text Between Curly Braces
	var str_C = "\n" + txt.value;
	var collectStr_C;
	var loopRes_C = "";
	
//		Loop To Loop Text Between {} inside an array
	
	while (collectStr_C = RegExp_C.exec(str_C)) { 
		arr_C.push(collectStr_C[1]);
	}
	
	for ( var a = 0 ; a < arr_C.length; a++) { 
				loopRes_C += "<div>" + "€" + arr_C[a] + "¥" + "</div>"
		}
	
//			Display Array Content

		
		res.innerHTML = loopRes_C;
		res.innerHTML = res.innerHTML.replace(/€/g , '$(".').replace(/¥/g , '");');
		
});
		
});

//	>>>>>>>>>>> $Btn3 <<<<<<<<<<<<


jqId.addEventListener("click", function () { 
	sub.className = "myJQId";
	
	desk.innerHTML =  'This option allows you to put selectors inside $("#selector") - this option can save many time for you to declare selectors inside variables and use them like you want in your jQuery Code ' + "<div style='padding: 30px'><i class='bold'>#Note</i></div>" + "your selectors should to be separated by dot and new line like the following Example" + "<ul style='margin-top: 10px;text-align:left'>" + 
	"<li>#selector1</li>" + 
	"<li>#selector2</li>" + 
	"<li>#selector3</li>" + 
	"<li>#etc__</li>" +
	"</ul>";
	
	var myJQId = document.getElementsByClassName("myJQId")[0];
	
	myJQId.addEventListener("click", function() { 
		
		var txt = document.getElementById("txt");
		var arr_D = []; // an array to collect the strings that are found
	var RegExp_D = /#(\w*)/g; // To Select All Text Between Curly Braces
	var str_D = "\n" + txt.value;
	var collectStr_D;
	var loopRes_D = "";
	
//		Loop To Loop Text Between {} inside an array
	
	while (collectStr_D = RegExp_D.exec(str_D)) { 
		arr_D.push(collectStr_D[1]);
	}
	
	for ( var a = 0 ; a < arr_D.length; a++) { 
				loopRes_D += "<div>" + "€" + arr_D[a] + "¥" + "</div>"
		}
	
//			Display Array Content

		
		res.innerHTML = loopRes_D;
		res.innerHTML = res.innerHTML.replace(/€/g , '$("#').replace(/¥/g , '");');
		
	});
		
});

//	>>>>>>>>>>>> Btn4 <<<<<<<<<<<<

jqMultiSelect.addEventListener("click", function() { 
	sub.className = "JQMultiSelectors";
	
	desk.innerHTML =  'This option allows you to put all selectors inside $("selector") - this option can save many time for you to declare selectors inside variables and use them like you want in your jQuery Code ' + "<div style='padding: 30px'><i class='bold'>#Note</i></div>" + "your selectors should to be separated by dot or hash and new line like the following Example" + "<ul style='margin-top: 10px;text-align:left'>" + 
	"<li>div</li>" + 
	"<li>#myId</li>" + 
	"<li>.myClass</li>" + 
	"<li>etc__</li>" +
	"</ul>" ;
	
	
	var JQMultiSelectors = document.getElementsByClassName("JQMultiSelectors")[0];
	
	JQMultiSelectors.addEventListener("click", function() { 
	
		txt.value = "\n" + txt.value;
		var myNewArr = [];
		var newTargetTxt = txt.value.match(/\n.*/g);
		var jqAllSelectorsLoop = "";
		for (var k = 0; k < newTargetTxt.length; k++) {
	 		myNewArr.push(newTargetTxt[k]);
	 		jqAllSelectorsLoop += '<div class="curlyLoopClass">' + "$(\"" + newTargetTxt[k] + "\");" + '</div>';
	}
	var kk = myNewArr;
	res.innerHTML = jqAllSelectorsLoop; 
	res.innerText = res.innerText.replace(/\n/g, "").replace(/\$/g , "\n$");; //jqAllSelectorsLoop;
	});
		
});


/*						JavaScript options					*/


//	>>>>>>>>>>> =Btn1 <<<<<<<<<<<<

jsTag.addEventListener("click", function() { 
	sub.className = "ESTag";
	
	
	desk.innerHTML =  'This option allows you to put tags name inside document.getElementsByTagName("tagName")[0] - by default we put the [index] if you want to remove this index there\'s Button after result you can remove it by click on this Button - this option can save many time for you to declare selectors inside variables and use them like you want in your JS Code ' +
	"<div style='padding: 30px'>" + 
		"<i class='bold'>#Note</i>" + 
	"</div>" + 
	"your selectors should to be separated by new line like the following Example" + 
	"<ul style='margin-top: 10px;text-align:left'>" + 
	"<li>body</li>" + 
	"<li>div</li>" + 
	"<li>h1</li>" + 
	"<li>etc__</li>" +
	"</ul>" ;
	
	var ESTag = document.getElementsByClassName("ESTag")[0];
	
	ESTag.addEventListener("click", function() { 
		
		txt.value = txt.value.replace(/\t/g, "").replace(/\s\t/g, "").replace(/\n/g , "£").replace(/\t\s/g, "").replace(/\n/g, "£").replace(/£{1,100}/g, "£");;
	txt.value = "£" + txt.value;
	
		var arrJSTag = []; // an array to collect the strings that are found
	var RegExpJSTag = /£(\w*)/g; // To Select All Text Between Curly Braces
	var strJSTag = txt.value;
	var collectStrJSTag;
	var loopResJSTag= "";
	
//		Loop To Loop Text Between {} inside an array
	
	while (collectStrJSTag = RegExpJSTag.exec(strJSTag)) { 
		arrJSTag.push(collectStrJSTag[1]);
	}
	
//			Display Array Content

		
		for ( var i = 0 ; i < arrJSTag.length; i++) { 
				loopResJSTag += "<div>" + "€" + arrJSTag[i] + "¥" + "</div>"
		}
		res.innerHTML = loopResJSTag;
		res.innerHTML = res.innerText.replace(/€/g , 'document.getElementsByTagName("').replace(/¥/g , '")[0];').replace(/document.getElementsByTagName\(\"\"\)\[0\];/g, "").replace(removeEmptyLines, "").replace(/;/g, ";\n");
	
		
	});
	
});

//	>>>>>>>>>>> =Btn2 <<<<<<<<<<<<

jsClass.addEventListener("click", function () { 
	sub.className = "ESClass";
	
	desk.innerHTML =  'This option allows you to put your class selectors inside document.getElementsByClassName("className")[0] - by default we put the [index] if you want to remove this index use the remove index Button after your result you - you can alse romove the semicolon to use it without declaring variables' + "<div class=\"bold\">Features</div>" +  'this option can save many time for you to declare selectors inside variables and use to them like you want in your JS Code ' +
	"<div style='padding: 30px'>" + 
		"<i class='bold'>#Note</i>" + 
	"</div>" + 
	"your selectors should to be separated by dot + new line like the following Example" + 
	"<ul style='margin-top: 10px;text-align:left'>" + 
	"<li>.class1</li>" + 
	"<li>.class2</li>" + 
	"<li>.class3</li>" + 
	"<li>etc__</li>" +
	"</ul>" ;
	
	var ESClass = document.getElementsByClassName("ESClass")[0];
	
	ESClass.addEventListener("click", function() { 
		
		var txt = document.getElementById("txt");
		var arrJSClass = []; // an array to collect the strings that are found
	var RegExpJSClass = /\n\.(\w*)/g; // To Select All Text Between Curly Braces
	var strJSClass = "\n" + txt.value;
	var collectStrJSClass;
	var loopResJSClass = "";
	
//		Loop To Loop Text Between {} inside an array
	
	while (collectStrJSClass = RegExpJSClass.exec(strJSClass)) { 
		arrJSClass.push(collectStrJSClass[1]);
	}
	
	for ( var a = 0 ; a < arrJSClass.length; a++) { 
				loopResJSClass += "<div>" + "€" + arrJSClass[a] + "¥" + "</div>"
		}
	
//			Display Array Content

		
		res.innerHTML = loopResJSClass;
		res.innerHTML = res.innerHTML.replace(/€/g , 'document.getElementsByClassName("').replace(/¥/g , '")[0];');
		
	});

});

//	>>>>>>>>>>> =Btn3 <<<<<<<<<<<<

jsId.addEventListener("click", function () { 
	sub.className = "ES_Id";

	desk.innerHTML =  'This option allows you to put your class selectors inside document.getElementsById(\"id\") - if you want romove the semi colon to use it without declaring variables use The Button after Your Result ' + "<div class=\"bold\">Features</div>" +  'this option save many time for you to declare HTML Selectors inside variables and use to them like you want in your script ' +
	"<div style='padding: 30px'>" + 
		"<i class='bold'>#Note</i>" + 
	"</div>" + 
	"your selectors should to be separated by #hash + new line like the following Example" + 
	"<ul style='margin-top: 10px;text-align:left'>" + 
	"<li>#id1</li>" + 
	"<li>#id2</li>" + 
	"<li>#id3</li>" + 
	"<li>etc__</li>" +
	"</ul>" ;
	
	var ES_Id = document.getElementsByClassName("ES_Id")[0];
	
	
		ES_Id.addEventListener("click", function() { 
		
		var arrESId = []; // an array to collect the strings that are found
	var RegExpESId = /#(\w*)/g; // To Select All Text Between Curly Braces
	var strESId = "\n" + txt.value;
	var collectStrESId;
	var loopResESId = "";
	
//		Loop To Loop Text Between {} inside an array
	
	while (collectStrESId = RegExpESId.exec(strESId)) { 
		arrESId.push(collectStrESId[1]);
	}
	
	for ( var a = 0 ; a < arrESId.length; a++) { 
				loopResESId += "<div>" + "€" + arrESId[a] + "¥" + "</div>"
		}
	
//			Display Array Content

		
		res.innerHTML = loopResESId;
		res.innerHTML = res.innerHTML.replace(/€/g , 'document.getElementById("').replace(/¥/g , '");');;
		
	});

});

/*						JS & jQuery options					*/


//	>>>>>>>>>>> &Btn1 <<<<<<<<<<<<


//	>>>>>>>>>>> &Btn2 <<<<<<<<<<<<

jqConvert.addEventListener("click", function () { 
	
	sub.className = "jQueryConvert";

	desk.innerHTML =  'This option allows you to convert your HTML code to use it in jQuery append Elements - just put your html doc in textbox and get your result ';
	
	var jQueryConvert = document.getElementsByClassName("jQueryConvert")[0];
	jQueryConvert.addEventListener("click", function() { 
			
		/*	txt.style.whiteSpace = "nowrap";
			res.style.whiteSpace = "nowrap;*/
			var removeQuoteSpaces = new RegExp("\t" , "g");
		var removeFirst2Char = new RegExp("^...", "g");
		var removeLast2Char = new RegExp("....$", "g")
		
		txt.innerText = txt.innerHTML;
		res.innerText = txt.value.replace(/<br>/g, "").replace(/"/g, "'").replace(/</g, "\" + \"<").replace(/>/g, ">\" + \"").replace(removeQuoteSpaces , "").replace(/\+ \"\"/g , "").replace(/\+ \"\n\"/g , "").replace(/\+ \"\t\"/g , "").replace(removeFirst2Char, "").replace(removeLast2Char, "")
			
	});

});


		</script>
		
		
		
		
		
		<!--


<div id="menu" class="menuCon">
				<div class="times">
					<i class="fas fa-times"></i>
				</div>
				<div class="dontWrap">
				<a href="#" class="menuLink link1">Home</a>
				<a href="#" class="menuLink link1">Services</a>
				<a href="#" class="menuLink link1">Tems</a>
				<a href="#" class="menuLink link1">Contact Us</a>
				<a href="#" class="menuLink link1">About Us</a>
				</div>
			</div> 

//Don't forget to search for way to replace regex with regex like replace [0-9] , [٠-٩]








/* '<div>"#Note: it it\'s Works Fine Now For Class , Id Only Now - if you used tags name may be you find some errors in your result"</div>' + 
	'<div>"#Note2: you can\'t use id only or tag name only you should write id + classes in the textbox to find your result "</div>'*/ 




/*var targetStr =  txt.value;
 		var tagsArr = []; 
		var idArr = []; 
		var classArr = []; 
	var tags_RegEx = /\n(\w*)/g;
	var id_RegEx = /#(\w*)/g;
	var class_RegEx = /\.(\w*)/g; 
	var tags_collectStr;
	var id_collectStr;
	var class_collectStr;
	var tags_Loop = "";
	var id_Loop = "";
	var class_Loop = "";
	
//		Loop To Loop Text Between {} inside an array
	
	while (tags_collectStr = tags_RegEx.exec(targetStr)) { 
		tagsArr.push(tags_collectStr[1]);
	}
	while (id_collectStr = id_RegEx.exec(targetStr)) { 
		idArr.push(id_collectStr[1]);
	}
	while (class_collectStr = class_RegEx.exec(targetStr)) { 
		classArr.push(class_collectStr[1]);
	}
	
	for ( var increase_A = 0, increase_B = 0, increase_C = 0 ; increase_A < tagsArr.length, increase_B < idArr.length, increase_C < classArr.length; increase_A++, increase_B++ , increase_C++) { 
				tags_Loop +=   "<div>" + "€" + tagsArr[increase_A] + "¥" + "</div>";
				id_Loop += "<div>" + "€#" + idArr[increase_B] + "¥" + "</div>";
				class_Loop += "<div>" + "€."+ classArr[increase_C] + "¥" + "</div>"
		}
	
//			Display Array Content

		
		res.innerHTML = tags_Loop.concat + id_Loop + class_Loop;
		res.innerHTML = res.innerHTML.replace(/€/g , '$("').replace(/¥/g , '");');*/


		
		-->
		
		




	 </body>
 </html>
