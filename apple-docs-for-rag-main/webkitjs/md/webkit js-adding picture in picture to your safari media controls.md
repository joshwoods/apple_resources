

- WebKit JS
-  Adding Picture in Picture to your Safari media controls 

Article

# Adding Picture in Picture to your Safari media controls

Create a custom control that adds Picture in Picture to your Safari media player.

## Overview

Although default controls are available for audio and video elements in your Safari webpage, you can also create your own custom media controls. One of the custom controls you should add is Picture in Picture. With Picture in Picture, your video remains in view in a floating video overlay while users interact with other apps.

### Write markup for a custom control

In this example, the custom controls for a video have only a Play button and a hidden Pause button:

&lt;video id=&quot;video&quot; src=&quot;my-video.mp4&quot;>&lt;/video>
&lt;div id=&quot;controls&quot;>
    &lt;button id=&quot;playButton&quot;>Play&lt;/button>
    &lt;button id=&quot;pauseButton&quot; hidden>Pause&lt;/button>
&lt;/div>

### Add a Picture-in-Picture element to your markup

Add markup for a new Picture-in-Picture button, which is visible by default.

&lt;video id=&quot;video&quot; src=&quot;my-video.mp4&quot;>&lt;/video>
&lt;div id=&quot;controls&quot;>
    &lt;button id=&quot;playButton&quot;>Play&lt;/button>
    &lt;button id=&quot;pauseButton&quot; hidden>Pause&lt;/button>
    &lt;button id=&quot;PiPButton&quot;>PiP&lt;/button>
&lt;/div> 

### Add functionality to the button

Add a function to toggle Picture in Picture using the webkitSetPresentationMode property from the presentation mode API.

if (video.webkitSupportsPresentationMode &amp;&amp; video.webkitSupportsPresentationMode(&quot;picture-in-picture&quot;) &amp;&amp; typeof video.webkitSetPresentationMode === &quot;function&quot;) {
    // Toggle PiP when the user clicks the button.
    pipButtonElement.addEventListener(&quot;click&quot;, function(event) {
        video.webkitSetPresentationMode(video.webkitPresentationMode === &quot;picture-in-picture&quot; ? &quot;inline&quot; : &quot;picture-in-picture&quot;);
    });
} else {
    pipButtonElement.disabled = true;
}

## See Also

### Essentials

Adding an AirPlay button to your Safari media controls

Create a custom control that adds AirPlay to your Safari media player.

