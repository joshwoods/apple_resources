

- Quartz
- IKSlideshow
-  run(with:inMode:options:) 

Instance Method

# run(with:inMode:options:)

Runs a slideshow that contains the specified kind of items, provided from a data source.

macOS 10.4+

``` source
func run(
    with dataSource: (any IKSlideshowDataSource)!,
    inMode slideshowMode: String!,
    options slideshowOptions: [AnyHashable : Any]! = [:]
)
```

## Parameters 

`dataSource`  

The data source to use for the slideshow.

`slideshowMode`  

A constant that indicate what kind of items are in the slideshow—`IKSlideshowModeImages`, `IKSlideshowModePDF`, or `IKSlideshowModeQuickLook`. See Slideshow Modes.

`slideshowOptions`  

A dictionary of slideshow options. See Slideshow Option Keys.

## See Also

### Running and Stopping a Slideshow

func stop(Any!)

Stops a slideshow.

var autoPlayDelay: TimeInterval

Controls the interval of time before a slideshow starts to play automatically.

