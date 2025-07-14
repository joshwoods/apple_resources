

- UIKit
- UINavigationBar
-  backgroundImage(for:) 

Instance Method

# backgroundImage(for:)

Returns the background image for given bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func backgroundImage(for barMetrics: UIBarMetrics) -> UIImage?
```

## Parameters 

`barMetrics`  

A bar metrics constant.

## Return Value

The background image for `barMetrics`.

## Discussion

Equivalent to using backgroundImage(for:barMetrics:) with a position of UIBarPosition.any.

## See Also

### Changing the background

var barTintColor: UIColor?

The tint color to apply to the navigation bar background.

func setBackgroundImage(UIImage?, for: UIBarMetrics)

Sets the background image for given bar metrics.

func backgroundImage(for: UIBarPosition, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image to use for a given bar position and set of metrics.

func setBackgroundImage(UIImage?, for: UIBarPosition, barMetrics: UIBarMetrics)

Sets the background image to use for a given bar position and set of metrics.

