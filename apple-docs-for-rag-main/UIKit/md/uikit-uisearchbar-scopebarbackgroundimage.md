

- UIKit
- UISearchBar
-  scopeBarBackgroundImage 

Instance Property

# scopeBarBackgroundImage

The background image for the scope bar.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var scopeBarBackgroundImage: UIImage? { get set }
```

## Discussion

Images that are 1 point wide or stretchable images are stretched, otherwise the image is tiled.

## See Also

### Related Documentation

var backgroundImage: UIImage?

The background image for the search bar.

### Customizing the scope bar appearance

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

func setScopeBarButtonTitleTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Sets the text attributes for the search bar’ button’s title string for a given state.

