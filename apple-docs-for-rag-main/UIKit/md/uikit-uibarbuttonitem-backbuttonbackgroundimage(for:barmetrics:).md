

- UIKit
- UIBarButtonItem
-  backButtonBackgroundImage(for:barMetrics:) 

Instance Method

# backButtonBackgroundImage(for:barMetrics:)

Returns the back button background image for a specified control state and bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func backButtonBackgroundImage(
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

The back button background image for `state` and `barMetrics`.

## Discussion

This modifier applies only to navigation bar back buttons and is ignored by other buttons.

## See Also

### Customizing the Back button

func setBackButtonBackgroundImage(UIImage?, for: UIControl.State, barMetrics: UIBarMetrics)

Sets the back button background image for a specified control state and bar metrics.

func backButtonTitlePositionAdjustment(for: UIBarMetrics) -> UIOffset

Returns the back button title offset for specified bar metrics.

func setBackButtonTitlePositionAdjustment(UIOffset, for: UIBarMetrics)

Sets the back button title offset for specified bar metrics.

func backButtonBackgroundVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the back button vertical position offset for specified bar metrics.

func setBackButtonBackgroundVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the back button vertical position offset for specified bar metrics.

