

- UIKit
- UIBarButtonItem
-  backgroundImage(for:barMetrics:) 

Instance Method

# backgroundImage(for:barMetrics:)

Returns the background image for a specified state and bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func backgroundImage(
    for state: UIControl.State,
    barMetrics: UIBarMetrics
) -> UIImage?
```

## Parameters 

`state`  

A control state.

`barMetrics`  

Bar metrics.

## Return Value

The background image for the button given state and metrics.

## See Also

### Customizing the background

func backgroundVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the background vertical position offset for specified bar metrics.

func setBackgroundVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the background vertical position offset for specified bar metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, barMetrics: UIBarMetrics)

Sets the background image for a specified state and bar metrics.

func backgroundImage(for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for the specified state, style, and metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics)

Sets the background image for the specified state, style, and metrics.

