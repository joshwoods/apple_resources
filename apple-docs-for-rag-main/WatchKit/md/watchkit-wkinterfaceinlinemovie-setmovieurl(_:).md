

- WatchKit
- WKInterfaceInlineMovie
-  setMovieURL(\_:) 

Instance Method

# setMovieURL(\_:)

Sets the URL of the movie to play.

watchOS 3.0+

``` source
func setMovieURL(_ URL: URL)
```

## Parameters 

`URL`  

The URL of the movie to play. The URL must be a file-based URL that refers to a movie or audio file in the appropriate format.

The URL must be in a shared location that can be accessed by both the Watch app interface and the WatchKit extension. For more information, see Sharing Data in App Programming Guide for watchOS.

## Discussion

Movies must be local to the device before playback begins. If you specify a URL that is on a remote server, Apple Watch downloads the movie before playing it.

## See Also

### Setting Movie Properties

func setAutoplays(Bool)

Sets a Boolean value indicating whether the movie automatically begins playing as soon as the scene is presented.

func setLoops(Bool)

Sets a Boolean value indicating whether the movie plays in a continuous loop.

func setPosterImage(WKImage?)

Sets the poster image to display for the movie.

func setVideoGravity(WKVideoGravity)

Sets the resizing behavior for the movie content.

