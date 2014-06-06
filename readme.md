# jquery-ga-playlength
PlayLength is a Google Analytics plugin that tracks how much of a HTML5 audio/video player a visitor plays. The plugin supports Universal Analytics, Classic Google Analytics, and Google Tag Manager.

## usage
The two requirements are Google Analytics and jQuery (v1.7+). Load the plugin and initialize Scroll Depth as in the example below. Make sure to place the initialization code after your Google Analytics tracking snippet.

	<script src="jquery.ga-playlength.min.js"></script>
	<script>
	$(function() {
		$('audio').gaPlayLength({
			/* audioTime: if true, the time in seconds of the 
			 * audio will be included wit the event. Default: true */
	        audioTime: true,
			/* userTiming: if true, the time in seconds since page load 
			 * will be included in the event. Default: true */
	        userTiming: true
	    });
	});
	</script>


## example
See `example.html`.

## thanks
Thanks to Rob Flaherty ([@robflaherty](https://twitter.com/robflaherty)) who created [jquery-scrolldepth](https://github.com/robflaherty/jquery-scrolldepth), which this PlayLength derived from.

## license
Licensed under the BSD 3-clause license, see `license.md`. See `jquery.ga-playlength.js` for dependency licenses.