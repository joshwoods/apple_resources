

- UIKit
- UISearchBar
-  setScopeBarButtonBackgroundImage(\_:for:) 

Instance Method

# setScopeBarButtonBackgroundImage(\_:for:)

Sets the background image for the scope bar button in a given state.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setScopeBarButtonBackgroundImage(
    _ backgroundImage: UIImage?,
    for state: UIControl.State
)
```

## Parameters 

`backgroundImage`  

The background image for the scope bar button in `state`.

`state`  

A control state.

## Discussion

For more details, see scopeBarButtonBackgroundImage(for:).

## See Also

### Customizing the scope bar appearance

var scopeBarBackgroundImage: UIImage?

The background image for the scope bar.

func scopeBarButtonBackgroundImage(for: UIControl.State) -> UIImage?

Returns the background image for the scope bar button in a given state.

func scopeBarButtonDividerImage(forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State) -> UIImage?

Returns the divider image to use for a given combination of left and right segment states.

func setScopeBarButtonDividerImage(UIImage?, forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State)

Sets the divider image to use for a given combination of left and right segment states.

func scopeBarButtonTitleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the text attributes for the search bar’s button’s title string for a given state.

func setScopeBarButtonTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes for the search bar’ button’s title string for a given state.

