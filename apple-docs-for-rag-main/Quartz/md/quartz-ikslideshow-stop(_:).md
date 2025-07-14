

- Quartz
- IKSlideshow
-  stop(\_:) 

Instance Method

# stop(\_:)

Stops a slideshow.

macOS 10.4+

``` source
func stop(_ sender: Any!)
```

## Parameters 

`sender`  

The object sending the message to stop the slideshow.

## Discussion

This method is invoked when the user clicks a button or issues a stop command.

## See Also

### Running and Stopping a Slideshow

func run(with: (any IKSlideshowDataSource)!, inMode: String!, options: [AnyHashable : Any]!)

Runs a slideshow that contains the specified kind of items, provided from a data source.

var autoPlayDelay: TimeInterval

Controls the interval of time before a slideshow starts to play automatically.

