

- UIKit
- UISearchBar
-  setScopeBarButtonTitleTextAttributes(\_:for:) 

Instance Method

# setScopeBarButtonTitleTextAttributes(\_:for:)

Sets the text attributes for the search bar’ button’s title string for a given state.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setScopeBarButtonTitleTextAttributes(
    _ attributes: [NSAttributedString.Key : Any]?,
    for state: UIControl.State
)
```

## Parameters 

`attributes`  

A dictionary containing key-value pairs specifying the text attributes to use for `state`.

You may specify the font, text color, text shadow color, and text shadow offset, using the keys found in NSString UIKit Additions Reference.

`state`  

A control state.

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

func setScopeBarButtonDividerImage(UIImage?, forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State)

Sets the divider image to use for a given combination of left and right segment states.

func scopeBarButtonTitleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the text attributes for the search bar’s button’s title string for a given state.

