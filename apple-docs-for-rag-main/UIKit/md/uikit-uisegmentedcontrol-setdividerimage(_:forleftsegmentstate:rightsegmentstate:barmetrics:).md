

- UIKit
- UISegmentedControl
-  setDividerImage(\_:forLeftSegmentState:rightSegmentState:barMetrics:) 

Instance Method

# setDividerImage(\_:forLeftSegmentState:rightSegmentState:barMetrics:)

Sets the divider image to use for a given combination of left and right segment states and bar metrics.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setDividerImage(
    _ dividerImage: UIImage?,
    forLeftSegmentState leftState: UIControl.State,
    rightSegmentState rightState: UIControl.State,
    barMetrics: UIBarMetrics
)
```

## Parameters 

`dividerImage`  

The divider image to use.

`leftState`  

The state of the left segment.

`rightState`  

The state of the right segment.

`barMetrics`  

Bar metrics.

## Discussion

To customize the segmented control appearance, provide divider images for the following cases:

- Between two unselected segments, where `leftState` and `rightState` are both normal

- Between a selected segment on the left and an unselected on the right, where `leftState` is selected and `rightState` is normal

- Between an unselected segment on the left and a selected on the right, where `leftState` is normal and `rightState` is selected

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

func dividerImage(forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State, barMetrics: UIBarMetrics) -> UIImage?

Returns the divider image used for a given combination of left and right segment states and bar metrics.

func titleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the text attributes of the title for a given control state.

func setTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes of the title for a given control state.

