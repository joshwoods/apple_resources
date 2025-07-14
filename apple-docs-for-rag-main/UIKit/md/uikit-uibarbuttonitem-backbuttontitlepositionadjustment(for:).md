

- UIKit
- UIBarButtonItem
-  backButtonTitlePositionAdjustment(for:) 

Instance Method

# backButtonTitlePositionAdjustment(for:)

Returns the back button title offset for specified bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func backButtonTitlePositionAdjustment(for barMetrics: UIBarMetrics) -> UIOffset
```

## Parameters 

`barMetrics`  

Bar metrics.

## Return Value

The back button title offset for `barMetrics`.

## Discussion

This modifier applies only to navigation bar back buttons and is ignored by other buttons.

## See Also

### Customizing the Back button

func backButtonBackgroundImage(for: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the back button background image for a specified control state and bar metrics.

func setBackButtonBackgroundImage(UIImage?, for: UIControl.State, barMetrics: UIBarMetrics)

Sets the back button background image for a specified control state and bar metrics.

func setBackButtonTitlePositionAdjustment(UIOffset, for: UIBarMetrics)

Sets the back button title offset for specified bar metrics.

func backButtonBackgroundVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the back button vertical position offset for specified bar metrics.

func setBackButtonBackgroundVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the back button vertical position offset for specified bar metrics.

