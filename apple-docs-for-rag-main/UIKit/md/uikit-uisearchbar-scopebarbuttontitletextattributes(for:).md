

- UIKit
- UISearchBar
-  scopeBarButtonTitleTextAttributes(for:) 

Instance Method

# scopeBarButtonTitleTextAttributes(for:)

Returns the text attributes for the search bar’s button’s title string for a given state.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func scopeBarButtonTitleTextAttributes(for state: UIControl.State) -> [NSAttributedString.Key : Any]?
```

## Parameters 

`state`  

A control state.

## Return Value

The text attributes for the search bar’ button’s title string for `state`.

The attributes may specify the font, text color, text shadow color, and text shadow offset, using the keys found in NSString UIKit Additions Reference.

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

func setScopeBarButtonTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes for the search bar’ button’s title string for a given state.

