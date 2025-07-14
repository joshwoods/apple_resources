

- WatchKit
- WKInterfaceInlineMovie
-  setVideoGravity(\_:) 

Instance Method

# setVideoGravity(\_:)

Sets the resizing behavior for the movie content.

watchOS 3.0+

``` source
func setVideoGravity(_ videoGravity: WKVideoGravity)
```

## Parameters 

`videoGravity`  

The resizing option for the movie. For a list of possible values, see the WKVideoGravity type. Defaults to WKVideoGravity.resizeAspect.

## See Also

### Setting Movie Properties

func setAutoplays(Bool)

Sets a Boolean value indicating whether the movie automatically begins playing as soon as the scene is presented.

func setLoops(Bool)

Sets a Boolean value indicating whether the movie plays in a continuous loop.

func setMovieURL(URL)

Sets the URL of the movie to play.

func setPosterImage(WKImage?)

Sets the poster image to display for the movie.

