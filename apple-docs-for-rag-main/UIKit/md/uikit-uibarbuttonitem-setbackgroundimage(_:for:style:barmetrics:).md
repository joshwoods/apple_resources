

- UIKit
- UIBarButtonItem
-  setBackgroundImage(\_:for:style:barMetrics:) 

Instance Method

# setBackgroundImage(\_:for:style:barMetrics:)

Sets the background image for the specified state, style, and metrics.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setBackgroundImage(
    _ backgroundImage: UIImage?,
    for state: UIControl.State,
    style: UIBarButtonItem.Style,
    barMetrics: UIBarMetrics
)
```

## Parameters 

`backgroundImage`  

The background image to use for the specified state, style, and metrics.

`state`  

The bar button state.

`style`  

The bar button style.

`barMetrics`  

The bar button metrics.

## Discussion

For good results, `backgroundImage` must be a stretchable image.

## See Also

### Customizing the background

func backgroundVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the background vertical position offset for specified bar metrics.

func setBackgroundVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the background vertical position offset for specified bar metrics.

func backgroundImage(for: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for a specified state and bar metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, barMetrics: UIBarMetrics)

Sets the background image for a specified state and bar metrics.

func backgroundImage(for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for the specified state, style, and metrics.

