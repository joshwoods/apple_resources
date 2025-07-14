

- WatchKit
- WKInterfaceMovie
-  setPosterImage(\_:) 

Instance Method

# setPosterImage(\_:)

Sets the poster image to display for the movie.

watchOS 2.0+

``` source
func setPosterImage(_ posterImage: WKImage?)
```

## Parameters 

`posterImage`  

The image to be displayed. Specifying `nil` removes the existing image, causing the watch interface to display nothing in the space previously occupied by the image.

## Discussion

This method changes the poster image that is displayed for the movie.

## See Also

### Setting the Movie Attributes

func setMovieURL(URL)

Sets the URL of the movie to play.

func setVideoGravity(WKVideoGravity)

Sets the resizing behavior for the movie content.

func setLoops(Bool)

Sets a Boolean value indicating whether the movie plays in a continuous loop.

