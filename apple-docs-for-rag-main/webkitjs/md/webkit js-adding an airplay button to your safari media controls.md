

- WebKit JS
-  Adding an AirPlay button to your Safari media controls 

Article

# Adding an AirPlay button to your Safari media controls

Create a custom control that adds AirPlay to your Safari media player.

## Overview

Although default controls are available for audio and video elements in your Safari webpage, you can also create your own custom media controls. One of the custom controls you should add is an AirPlay button.

### Write markup for a custom control 

In this example, the custom controls for a video have only a Play button and a hidden Pause button:

&lt;video id=&quot;video&quot; src=&quot;my-video.mp4&quot;>&lt;/video>
&lt;div id=&quot;controls&quot;>
    &lt;button id=&quot;playButton&quot;>Play&lt;/button>
    &lt;button id=&quot;pauseButton&quot; hidden>Pause&lt;/button>
&lt;/div>

### Add an AirPlay element to your markup 

Add markup for the AirPlay button, setting it to hidden by default to mimic the behavior of the AirPlay button in default controls. The default button appears only when AirPlay is available.

&lt;video id=&quot;video&quot; src=&quot;my-video.mp4&quot;>&lt;/video>
&lt;div id=&quot;controls&quot;>
    &lt;button id=&quot;playButton&quot;>Play&lt;/button>
    &lt;button id=&quot;pauseButton&quot; hidden>Pause&lt;/button>
    &lt;button id=&quot;airPlayButton&quot; hidden disabled>AirPlay&lt;/button>
&lt;/div> 

### Add an event listener 

To show the AirPlay button when AirPlay is available, you add an event listener for the `webkitplaybacktargetavailabilitychanged` event. This event detects when AirPlay availability changes, and it changes the visibility of the AirPlay button from the above default markup.

Note

To conserve battery power, listen for this event only for as long as needed, and then stop listening. If the button is not visible, controls are hidden, or the user is in fullscreen mode, stop listening.

### Select the AirPlay device 

Add this block of code to use the native AirPlay route picker in your controls. With this route picker, you can add and select an available AirPlay device:

### Ensure that styles persist when playing over AirPlay 

Use the code below to listen for the event `webkitcurrentplaybacktargetiswirelesschanged`. This event fires when a media element starts or stops AirPlay playback. Use this event to update styles.

## See Also

### Essentials

Adding Picture in Picture to your Safari media controls

Create a custom control that adds Picture in Picture to your Safari media player.

