

- TVMLKit JS
- MediaItem
-  highlightGroups 

Instance Property

# highlightGroups

An array of highlight groups, with each group containing a list of highlights.

tvOS 9.0+

``` source
attribute Array highlightGroups;
```

## Discussion

The `highlightGroups` property enables you to show several groups of highlights from a stream. Each highlight group in the array contains a list of highlights. Each highlight is an object with the following properties: `description`, `duration`, `imageURL`, `name`, and `starttime`. Highlight objects are ad-hoc JSON objects and there are no explicit classes for these types.

A good way to envision how the `highlightGroups` property works is to think of a video of a baseball game. During the game, several home runs are hit. You can create a highlight group containing the video for each of these highlights and put the highlight group into the `highlightGroups` property. Listing 1 shows a complete example of how to set up a highlight group.

var baseURL;

App.onLaunch = function(options) {
    baseURL = options.BASEURL;
    var documentPath = &quot;path to file on server/baseball.m3u8&quot;;
    var videourl = baseURL + documentPath;

    var singleVideo = new MediaItem(&#39;video&#39;, videourl);
    var highlights = [{
        name: &quot;Home Runs&quot;,
        highlights: [{
            name: &quot;Johnny Appleseed 1st inning&quot;,
            description: &quot;Johnny&#39;s 1st Homerun&quot;,
            starttime: 10,
            duration: 10,
            imageURL: &quot;path to server/images/Car_Movie_90x90_A.png&quot;
            },
        {
            name: &quot;Johnny Appleseed 5th inning&quot;,
            description: &quot;Johnny&#39;s 2nd Homerun&quot;,
            starttime: 60,
            duration: 10,
            imageURL: &quot;path to server/images/Car_Movie_90x90_B.png&quot;
            }
        ]
    }];
    singleVideo.highlightGroups = highlights;
    var videoList = new Playlist();
    videoList.push(singleVideo);
    var myPlayer = new Player();
    myPlayer.playlist = videoList;
    myPlayer.play();
}

App.onExit = function() {
    console.log(&quot;exited&quot;);
}

Listing 1 highlightGroups.js example

Note

You can only have one set of highlights associated with a media item.

## See Also

### Setting Timing Options

interstitials

An array of `interstitial` objects.

resumeTime

The number of seconds from the beginning of the item at which the item begins playing.

