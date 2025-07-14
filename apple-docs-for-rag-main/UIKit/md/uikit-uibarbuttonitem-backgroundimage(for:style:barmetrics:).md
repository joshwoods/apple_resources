

- UIKit
- UIBarButtonItem
-  backgroundImage(for:style:barMetrics:) 

Instance Method

# backgroundImage(for:style:barMetrics:)

Returns the background image for the specified state, style, and metrics.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func backgroundImage(
    for state: UIControl.State,
    style: UIBarButtonItem.Style,
    barMetrics: UIBarMetrics
) -> UIImage?
```

## Parameters 

`state`  

The bar button state.

`style`  

The bar button style.

`barMetrics`  

The bar button metrics.

## Return Value

The background image associated with the specified state, style, and metrics.

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

func setBackgroundImage(UIImage?, for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics)

Sets the background image for the specified state, style, and metrics.

