

- Quartz
- IKSlideshow
-  autoPlayDelay 

Instance Property

# autoPlayDelay

Controls the interval of time before a slideshow starts to play automatically.

macOS 10.4+

``` source
var autoPlayDelay: TimeInterval { get set }
```

## See Also

### Running and Stopping a Slideshow

func run(with: (any IKSlideshowDataSource)!, inMode: String!, options: [AnyHashable : Any]!)

Runs a slideshow that contains the specified kind of items, provided from a data source.

func stop(Any!)

Stops a slideshow.

