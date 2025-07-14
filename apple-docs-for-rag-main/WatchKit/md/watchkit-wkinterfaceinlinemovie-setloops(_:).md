

- WatchKit
- WKInterfaceInlineMovie
-  setLoops(\_:) 

Instance Method

# setLoops(\_:)

Sets a Boolean value indicating whether the movie plays in a continuous loop.

watchOS 3.0+

``` source
func setLoops(_ loops: Bool)
```

## Parameters 

`loops`  

A Boolean value indicating the looping behavior. Specify true to play the movie in a continuous loop or false to play the movie once and then stop playback. Defaults to false.

## See Also

### Setting Movie Properties

func setAutoplays(Bool)

Sets a Boolean value indicating whether the movie automatically begins playing as soon as the scene is presented.

func setMovieURL(URL)

Sets the URL of the movie to play.

func setPosterImage(WKImage?)

Sets the poster image to display for the movie.

func setVideoGravity(WKVideoGravity)

Sets the resizing behavior for the movie content.

