

- UIKit
- UINavigationBar
-  setBackgroundImage(\_:for:) 

Instance Method

# setBackgroundImage(\_:for:)

Sets the background image for given bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setBackgroundImage(
    _ backgroundImage: UIImage?,
    for barMetrics: UIBarMetrics
)
```

## Parameters 

`backgroundImage`  

The background image to use for `barMetrics`.

`barMetrics`  

A bar metrics constant.

## Discussion

Equivalent to using setBackgroundImage(_:for:barMetrics:) with a position of UIBarPosition.any.

## See Also

### Changing the background

var barTintColor: UIColor?

The tint color to apply to the navigation bar background.

func backgroundImage(for: UIBarMetrics) -> UIImage?

Returns the background image for given bar metrics.

func backgroundImage(for: UIBarPosition, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image to use for a given bar position and set of metrics.

func setBackgroundImage(UIImage?, for: UIBarPosition, barMetrics: UIBarMetrics)

Sets the background image to use for a given bar position and set of metrics.

