

- UIKit
- UIBarButtonItem
-  setBackgroundVerticalPositionAdjustment(\_:for:) 

Instance Method

# setBackgroundVerticalPositionAdjustment(\_:for:)

Sets the background vertical position offset for specified bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setBackgroundVerticalPositionAdjustment(
    _ adjustment: CGFloat,
    for barMetrics: UIBarMetrics
)
```

## Parameters 

`adjustment`  

The background vertical position offset for `barMetrics`.

`barMetrics`  

Bar metrics.

## Discussion

This offset is used to adjust the vertical centering of bordered bar buttons within the bar.

## See Also

### Customizing the background

func backgroundVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the background vertical position offset for specified bar metrics.

func backgroundImage(for: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for a specified state and bar metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, barMetrics: UIBarMetrics)

Sets the background image for a specified state and bar metrics.

func backgroundImage(for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for the specified state, style, and metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, style: UIBarButtonItem.Style, barMetrics: UIBarMetrics)

Sets the background image for the specified state, style, and metrics.

