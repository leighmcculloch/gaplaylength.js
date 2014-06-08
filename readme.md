# jquery-ga-playlength
A Google Analytics plugin that measures engagement in audio/video content by tracking how much of a HTML5 audio/video player a visitor plays. The plugin supports Universal Analytics, Classic Google Analytics, and Google Tag Manager.

The following time portions are reported:  
* Baseline — triggered when playing  
* 10%
* 50%
* 75%
* 100% — triggered when the playing ends

The above items are only triggered once for the audio/video element.

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