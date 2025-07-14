

- UIKit
- UIBarButtonItem
-  setBackButtonBackgroundImage(\_:for:barMetrics:) 

Instance Method

# setBackButtonBackgroundImage(\_:for:barMetrics:)

Sets the back button background image for a specified control state and bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
func setBackButtonBackgroundImage(
    _ backgroundImage: UIImage?,
    for state: UIControl.State,
    barMetrics: UIBarMetrics
)
```

## Parameters 

`backgroundImage`  

The image to use for the back button’s background.

`state`  

A control state.

`barMetrics`  

Bar metrics.

## Discussion

This modifier applies only to navigation bar back buttons and is ignored by other buttons.

For good results, `backgroundImage` must be a stretchable image.

## See Also

### Customizing the Back button

func backButtonBackgroundImage(for: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the back button background image for a specified control state and bar metrics.

func backButtonTitlePositionAdjustment(for: UIBarMetrics) -> UIOffset

Returns the back button title offset for specified bar metrics.

func setBackButtonTitlePositionAdjustment(UIOffset, for: UIBarMetrics)

Sets the back button title offset for specified bar metrics.

func backButtonBackgroundVerticalPositionAdjustment(for: UIBarMetrics) -> CGFloat

Returns the back button vertical position offset for specified bar metrics.

func setBackButtonBackgroundVerticalPositionAdjustment(CGFloat, for: UIBarMetrics)

Sets the back button vertical position offset for specified bar metrics.

