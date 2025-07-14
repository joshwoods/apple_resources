

- UIKit
- UINavigationBar
-  setBackgroundImage(\_:for:barMetrics:) 

Instance Method

# setBackgroundImage(\_:for:barMetrics:)

Sets the background image to use for a given bar position and set of metrics.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setBackgroundImage(
    _ backgroundImage: UIImage?,
    for barPosition: UIBarPosition,
    barMetrics: UIBarMetrics
)
```

## Parameters 

`backgroundImage`  

The image to use for the specified location and metrics.

`barPosition`  

The location of the navigation bar.

`barMetrics`  

The metrics of the navigation bar.

## Discussion

Resizable images will be stretched vertically, if necessary, for a position of UIBarPosition.topAttached.

## See Also

### Changing the background

var barTintColor: UIColor?

The tint color to apply to the navigation bar background.

func backgroundImage(for: UIBarMetrics) -> UIImage?

Returns the background image for given bar metrics.

func setBackgroundImage(UIImage?, for: UIBarMetrics)

Sets the background image for given bar metrics.

func backgroundImage(for: UIBarPosition, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image to use for a given bar position and set of metrics.

