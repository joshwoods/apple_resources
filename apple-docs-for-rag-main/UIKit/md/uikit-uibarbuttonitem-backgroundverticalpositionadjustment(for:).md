

- UIKit
- UIBarButtonItem
-  backgroundVerticalPositionAdjustment(for:) 

Instance Method

# backgroundVerticalPositionAdjustment(for:)

Returns the background vertical position offset for specified bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func backgroundVerticalPositionAdjustment(for barMetrics: UIBarMetrics) -> CGFloat
```

## Parameters 

`barMetrics`  

Bar metrics.

## Return Value

The background vertical position offset for `barMetrics`.

## Discussion

This offset is used to adjust the vertical centering of bordered bar buttons within the bar.

## See Also

### Customizing the background

func setBackgroundVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the background vertical position offset for specified bar metrics.

func backgroundImage(for: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for a specified state and bar metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, barMetrics: UIBarMetrics)

Sets the background image for a specified state and bar metrics.

func backgroundImage(for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for the specified state, style, and metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics)

Sets the background image for the specified state, style, and metrics.

