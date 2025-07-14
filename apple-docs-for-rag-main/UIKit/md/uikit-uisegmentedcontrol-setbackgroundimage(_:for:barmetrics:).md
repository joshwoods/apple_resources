

- UIKit
- UISegmentedControl
-  setBackgroundImage(\_:for:barMetrics:) 

Instance Method

# setBackgroundImage(\_:for:barMetrics:)

Sets the background image for given state and bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setBackgroundImage(
    _ backgroundImage: UIImage?,
    for state: UIControl.State,
    barMetrics: UIBarMetrics
)
```

## Parameters 

`backgroundImage`  

The background image to use for `state` and `barMetrics`.

`state`  

A control state.

`barMetrics`  

Bar metrics.

## Discussion

If `backgroundImage` is an image that resizableImage(withCapInsets:) returns, the system calculates the cap widths from that information.

If `backgroundImage` isn’t an image that resizableImage(withCapInsets:) returns, the system calculates the cap width by subtracting one from the image’s width, then dividing by 2. The system uses the cap widths as the margins for text placement. To adjust the margin, use the margin adjustment methods.

Generally, specify a value for the normal state. The segmented control uses this state for other states that don’t have a custom value set.

Similarly, when a property is dependent on the bar metrics, be sure to specify a value for UIBarMetrics.default. The segmented control respects properties for UIBarMetrics.compact only when the control is in smaller navigation and toolbars.

## See Also

### Customizing appearance

var selectedSegmentTintColor: UIColor?

The color to use for highlighting the currently selected segment.

func backgroundImage(for: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for a given state and bar metrics.

func contentPositionAdjustment(forSegmentType: UISegmentedControl.Segment, barMetrics: UIBarMetrics) -> UIOffset

Returns the positioning offset for a given segment and bar metrics.

func setContentPositionAdjustment(UIOffset, forSegmentType: UISegmentedControl.Segment, barMetrics: UIBarMetrics)

Sets the content positioning offset for a given segment and bar metrics.

enum Segment

Constants for specifying a segment in a control.

func dividerImage(forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the divider image used for a given combination of left and right segment states and bar metrics.

func setDividerImage(UIImage?, forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State, barMetrics: UIBarMetrics)

Sets the divider image to use for a given combination of left and right segment states and bar metrics.

func titleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the text attributes of the title for a given control state.

func setTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes of the title for a given control state.

