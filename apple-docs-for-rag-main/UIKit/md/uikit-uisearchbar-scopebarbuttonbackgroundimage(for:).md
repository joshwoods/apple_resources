

- UIKit
- UISearchBar
-  scopeBarButtonBackgroundImage(for:) 

Instance Method

# scopeBarButtonBackgroundImage(for:)

Returns the background image for the scope bar button in a given state.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func scopeBarButtonBackgroundImage(for state: UIControl.State) -> UIImage?
```

## Parameters 

`state`  

A control state.

## Return Value

The background image for the scope bar button in `state`.

## Discussion

If the background image is an image returned from stretchableImage(withLeftCapWidth:topCapHeight:) (`UIImage`), the cap widths are calculated from that information, otherwise, the cap width is calculated by subtracting one from the image’s width then dividing by 2. The cap widths are used as the margins for text placement. To adjust the margin use the margin adjustment methods.

## See Also

### Customizing the scope bar appearance

var scopeBarBackgroundImage: UIImage?

The background image for the scope bar.

func setScopeBarButtonBackgroundImage(UIImage?, for: UIControl.State)

Sets the background image for the scope bar button in a given state.

func scopeBarButtonDividerImage(forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State) -> UIImage?

Returns the divider image to use for a given combination of left and right segment states.

func setScopeBarButtonDividerImage(UIImage?, forLeftSegmentState: UIControl.State, rightSegmentState: UIControl.State)

Sets the divider image to use for a given combination of left and right segment states.

func scopeBarButtonTitleTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the text attributes for the search bar’s button’s title string for a given state.

func setScopeBarButtonTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes for the search bar’ button’s title string for a given state.

