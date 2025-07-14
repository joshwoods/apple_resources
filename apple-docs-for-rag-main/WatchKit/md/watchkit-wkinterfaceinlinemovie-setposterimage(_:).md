

- WatchKit
- WKInterfaceInlineMovie
-  setPosterImage(\_:) 

Instance Method

# setPosterImage(\_:)

Sets the poster image to display for the movie.

watchOS 3.0+

``` source
func setPosterImage(_ posterImage: WKImage?)
```

## Parameters 

`posterImage`  

The image to be displayed. Specifying `nil` removes the existing image, causing the watch interface to display nothing in the space previously occupied by the image.

## Discussion

This method changes the poster image that is displayed for the movie.

## See Also

### Setting Movie Properties

func setAutoplays(Bool)

Sets a Boolean value indicating whether the movie automatically begins playing as soon as the scene is presented.

func setLoops(Bool)

Sets a Boolean value indicating whether the movie plays in a continuous loop.

func setMovieURL(URL)

Sets the URL of the movie to play.

func setVideoGravity(WKVideoGravity)

Sets the resizing behavior for the movie content.

