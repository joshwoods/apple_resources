

- UIKit
- UISearchBar
-  setScopeBarButtonDividerImage(\_:forLeftSegmentState:rightSegmentState:) 

Instance Method

# setScopeBarButtonDividerImage(\_:forLeftSegmentState:rightSegmentState:)

Sets the divider image to use for a given combination of left and right segment states.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setScopeBarButtonDividerImage(
    _ dividerImage: UIImage?,
    forLeftSegmentState leftState: UIControl.State,
    rightSegmentState rightState: UIControl.State
)
```

## Parameters 

`dividerImage`  

The divider image to use for the combination of `leftState` and `rightState`.

`leftState`  

The state of the left segment for which to set the divider image.

The state may be normal or selected.

`rightState`  

The state of the right segment for which to set the divider image.

The state may be normal or selected.

## Discussion

To customize the segmented control appearance you need to provide divider images to go between two unselected segments (`leftSegmentState:UIControlStateNormal rightSegmentState:UIControlStateNormal`), selected on the left and unselected on the right (`leftSegmentState:UIControlStateSelected rightSegmentState:UIControlStateNormal`), and unselected on the left and selected on the right (`leftSegmentState:UIControlStateNormal rightSegmentState:UIControlStateSelected`).

## See Also

### Customizing the scope bar appearance

var scopeBarBackgroundImage: UIImage?

The background image for the scope bar.

func scopeBarButtonBackgroundImage(for: UIControl.State) -> UIImage?

Returns the background image for the scope bar button in a given state.

func setScopeBarButtonBackgroundImage(UIImage?, for: UIControl.State)

Sets the background image for the scope bar button in a given state.

func scopeBarButtonDividerImage(forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State) -> UIImage?

Returns the divider image to use for a given combination of left and right segment states.

func scopeBarButtonTitleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the text attributes for the search bar’s button’s title string for a given state.

func setScopeBarButtonTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes for the search bar’ button’s title string for a given state.

