

- UIKit
- UIToolbar
-  backgroundImage(forToolbarPosition:barMetrics:) 

Instance Method

# backgroundImage(forToolbarPosition:barMetrics:)

Returns the image to use for the background in a given position and with given metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func backgroundImage(
    forToolbarPosition topOrBottom: UIBarPosition,
    barMetrics: UIBarMetrics
) -> UIImage?
```

## Parameters 

`topOrBottom`  

The location the bar is being drawn in.

`barMetrics`  

The metrics being used to draw the bar.

## Return Value

The image to use for the toolbar background in the position specified by `topOrBottom` and with the metrics specified by `barMetrics`.

## Discussion

The default value is `nil`. When non-`nil` the image will be used instead of the system image for toolbars in the specified position.

## See Also

### Changing the background

var barTintColor: UIColor?

The tint color to apply to the toolbar background.

func setBackgroundImage(UIImage?, forToolbarPosition: UIBarPosition, barMetrics: UIBarMetrics)

Sets the image to use for the background in a given position and with given metrics.

