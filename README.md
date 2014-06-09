# Continuous Reel Slideshow #

*Description:*  DD Mega Menu is the ideal menu script to use when you need a drop down menu system that supports arbitrary sub menu layouts, such as multiple columns of links or even arbitrary HTML. Each drop down menu is simply defined inline on the page as a regular DIV, making it extremely easy to customize its contents whichever way you like.

## Directions ##

*Step 1:* This script uses the following external files:

+ jQuery 1.5 or above (served via Google CDN)
+ ddmegamenu.js
+ ddmegamenu.css

*Step 2:* Add the below code to the HEAD section of your page:

	<script type="text/javascript" src="http://ajax.googleapis.com/ajax/libs/jquery/1.4.2/jquery.min.js"></script>
	<script type="text/javascript" src="jquery.touchSwipe.min.js"></script>
	
	<style type="text/css">
	
	#myreel{ /*sample CSS for demo*/
	border:15px solid black;
	}
	
	.paginate{
	width: 330px;
	margin-top:5px;
	font:bold 14px Arial;
	text-align:center;
	}
	
	</style>
	
	<script src="reelslideshow.js" type="text/javascript">
	
	/***********************************************
	* Continuous Reel Slideshow- © Dynamic Drive (www.dynamicdrive.com)
	* This notice MUST stay intact for legal use
	* Visit http://www.dynamicdrive.com/ for this script and 100s more.
	***********************************************/
	
	</script>
	
	<script type="text/javascript">
	
	var firstreel=new reelslideshow({
		wrapperid: "myreel", //ID of blank DIV on page to house Slideshow
		dimensions: [300, 200], //width/height of gallery in pixels. Should reflect dimensions of largest image
		imagearray: [
			["http://i26.tinypic.com/11l7ls0.jpg"], //["image_path", "optional_link", "optional_target"]
			["http://i29.tinypic.com/xp3hns.jpg", "http://en.wikipedia.org/wiki/Cave", "_new"],
			["http://i30.tinypic.com/531q3n.jpg"],
			["http://i31.tinypic.com/119w28m.jpg"] //<--no trailing comma after very last image element!
		],
		displaymode: {type:'auto', pause:2000, cycles:2, pauseonmouseover:true},
		orientation: "h", //Valid values: "h" or "v"
		persist: true, //remember last viewed slide and recall within same session?
		slideduration: 300 //transition duration (milliseconds)
	})
	
	</script>


*Step 3:* Then, add the below sample markup to your page:

	<div id="myreel"></div>
	
	<div class="paginate">
	<a href="javascript:firstreel.navigate('back')" style="margin-right:200px;">back</a>  <a href="javascript:firstreel.navigate('forth')">forth</a>
	</div>

## Continuous Reel Slideshow set up ##

See script project page for additional details on setup and documentation: <http://www.dynamicdrive.com/dynamicindex14/reelslideshow.htm>
