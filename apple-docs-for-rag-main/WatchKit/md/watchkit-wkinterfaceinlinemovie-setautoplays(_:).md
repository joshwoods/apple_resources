

- WatchKit
- WKInterfaceInlineMovie
-  setAutoplays(\_:) 

Instance Method

# setAutoplays(\_:)

Sets a Boolean value indicating whether the movie automatically begins playing as soon as the scene is presented.

watchOS 3.0+

``` source
func setAutoplays(_ autoplays: Bool)
```

## Parameters 

`autoplays`  

A Boolean value indicating the movie’s autoplay behavior. Specify true to have the movie automatically play as soon as the scene is presented. If set to false, the inline movie object displays the poster image instead. The movie does not begin playing until the user taps the poster, or until you programmatically call either the play() or playFromBeginning() method. Defaults to true.

## See Also

### Setting Movie Properties

func setLoops(Bool)

Sets a Boolean value indicating whether the movie plays in a continuous loop.

func setMovieURL(URL)

Sets the URL of the movie to play.

func setPosterImage(WKImage?)

Sets the poster image to display for the movie.

func setVideoGravity(WKVideoGravity)

Sets the resizing behavior for the movie content.

