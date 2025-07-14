

- TVMLKit JS
- MediaItem
-  interstitials 

Instance Property

# interstitials

An array of `interstitial` objects.

tvOS 9.0+

``` source
attribute Array interstitials;
```

## Discussion

An interstitial object defines a point within a `MediaItem` object where you can insert another media item; for example, a short ad. Each interstitial object in the array contains two keys: `starttime` and `duration`. The `starttime` is the length of time from the beginning of a media item, in seconds. The `duration` is the length of the interstitial, in seconds. Both keys are required. A common use for these objects is to define when and where ads are to be played during a stream. Listing 1 shows a complete TVMLKit JS example for incorporating interstitials. A single interstitial is defined. In addition, an event listener is created that prevents users from fast-forwarding or rewinding during the duration of the interstitial.

var baseURL;

App.onLaunch = function(options) {
    baseURL = options.BASEURL;
    var documentPath = &quot;path to file on server/baseball.m3u8&quot;;
    var videourl = baseURL + documentPath;

    var singleVideo = new MediaItem(&#39;video&#39;, videourl);
    var videoInterstitials = [];
    videoInterstitials.push({
        starttime: 30,
        duration: 20
    });
    singleVideo.interstitials = videoInterstitials;
    var videoList = new Playlist();
    videoList.push(singleVideo);
    var myPlayer = new Player();
    myPlayer.playlist = videoList;
    myPlayer.addEventListener(&quot;requestSeekToTime&quot;, function(event) {
        if (event.currentTime > 30 &amp;&amp; event.currentTime &lt;50) {return false;} else {return true;}
        });
    myPlayer.play();
}

App.onExit = function() {
    console.log(&quot;exited&quot;);
}

Listing 1 interstitials.js example

## See Also

### Setting Timing Options

highlightGroups

An array of highlight groups, with each group containing a list of highlights.

resumeTime

The number of seconds from the beginning of the item at which the item begins playing.

