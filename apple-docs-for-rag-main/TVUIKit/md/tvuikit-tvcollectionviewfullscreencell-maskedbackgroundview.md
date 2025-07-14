

- TVUIKit
- TVCollectionViewFullScreenCell
-  maskedBackgroundView 

Instance Property

# maskedBackgroundView

The background view that performs the parallax effect.

tvOS 13.0+

``` source
@MainActor
var maskedBackgroundView: UIView { get }
```

## Discussion

The `maskedBackgroundView` property returns the current cell’s background view. Modify properties of this view to customize the parallax effect. Generally, you should add an opaque image to the view.

## See Also

### Accessing Cell Views

var maskedContentView: UIView

The content view in focus.

