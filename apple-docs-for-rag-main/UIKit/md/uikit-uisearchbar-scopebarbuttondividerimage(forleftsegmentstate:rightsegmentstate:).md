

- UIKit
- UISearchBar
-  scopeBarButtonDividerImage(forLeftSegmentState:rightSegmentState:) 

Instance Method

# scopeBarButtonDividerImage(forLeftSegmentState:rightSegmentState:)

Returns the divider image to use for a given combination of left and right segment states.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func scopeBarButtonDividerImage(
    forLeftSegmentState leftState: UIControl.State,
    rightSegmentState rightState: UIControl.State
) -> UIImage?
```

## Parameters 

`leftState`  

The state of the left segment for which to provide the divider image.

The state may be normal or selected.

`rightState`  

The state of the right segment for which to provide the divider image.

The state may be normal or selected.

## Return Value

The divider image to use for the combination of `leftState` and `rightState`.

## Discussion

For more details, see setScopeBarButtonDividerImage(_:forLeftSegmentState:rightSegmentState:)

## See Also

### Customizing the scope bar appearance

var scopeBarBackgroundImage: UIImage?

The background image for the scope bar.

func scopeBarButtonBackgroundImage(for: UIControl.State) -> UIImage?

Returns the background image for the scope bar button in a given state.

func setScopeBarButtonBackgroundImage(UIImage?, for: UIControl.State)

Sets the background image for the scope bar button in a given state.

func setScopeBarButtonDividerImage(UIImage?, forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State)

Sets the divider image to use for a given combination of left and right segment states.

func scopeBarButtonTitleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the text attributes for the search bar’s button’s title string for a given state.

func setScopeBarButtonTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes for the search bar’ button’s title string for a given state.

