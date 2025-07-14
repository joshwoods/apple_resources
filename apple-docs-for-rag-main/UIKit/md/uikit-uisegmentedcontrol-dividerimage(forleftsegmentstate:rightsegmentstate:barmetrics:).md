

- UIKit
- UISegmentedControl
-  dividerImage(forLeftSegmentState:rightSegmentState:barMetrics:) 

Instance Method

# dividerImage(forLeftSegmentState:rightSegmentState:barMetrics:)

Returns the divider image used for a given combination of left and right segment states and bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func dividerImage(
    forLeftSegmentState leftState: UIControl.State,
    rightSegmentState rightState: UIControl.State,
    barMetrics: UIBarMetrics
) -> UIImage?
```

## Parameters 

`leftState`  

The state of the left segment.

`rightState`  

The state of the right segment.

`barMetrics`  

Bar metrics.

## Return Value

The divider image used for the given combination of left and right segment states and bar metrics

## See Also

### Customizing appearance

var selectedSegmentTintColor: UIColor?

The color to use for highlighting the currently selected segment.

func backgroundImage(for: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image for a given state and bar metrics.

func setBackgroundImage(UIImage?, for: UIControl.State, barMetrics: UIBarMetrics)

Sets the background image for given state and bar metrics.

func contentPositionAdjustment(forSegmentType: UISegmentedControl.Segment, barMetrics: UIBarMetrics) -> UIOffset

Returns the positioning offset for a given segment and bar metrics.

func setContentPositionAdjustment(UIOffset, forSegmentType: UISegmentedControl.Segment, barMetrics: UIBarMetrics)

Sets the content positioning offset for a given segment and bar metrics.

enum Segment

Constants for specifying a segment in a control.

func setDividerImage(UIImage?, forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State, barMetrics: UIBarMetrics)

Sets the divider image to use for a given combination of left and right segment states and bar metrics.

func titleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the text attributes of the title for a given control state.

func setTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes of the title for a given control state.

