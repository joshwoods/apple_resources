

- UIKit
- UIToolbar
-  setBackgroundImage(\_:forToolbarPosition:barMetrics:) 

Instance Method

# setBackgroundImage(\_:forToolbarPosition:barMetrics:)

Sets the image to use for the background in a given position and with given metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setBackgroundImage(
    _ backgroundImage: UIImage?,
    forToolbarPosition topOrBottom: UIBarPosition,
    barMetrics: UIBarMetrics
)
```

## Parameters 

`backgroundImage`  

The image to use for the toolbar background in the position specified by `topOrBottom` and with the metrics specified by `barMetrics`.

`topOrBottom`  

A toolbar position constant.

`barMetrics`  

A bar metrics constant.

## See Also

### Changing the background

var barTintColor: UIColor?

The tint color to apply to the toolbar background.

func backgroundImage(forToolbarPosition: UIBarPosition, barMetrics: UIBarMetrics) -> UIImage?

Returns the image to use for the background in a given position and with given metrics.

