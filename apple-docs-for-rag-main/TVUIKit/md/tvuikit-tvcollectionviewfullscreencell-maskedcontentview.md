

- TVUIKit
- TVCollectionViewFullScreenCell
-  maskedContentView 

Instance Property

# maskedContentView

The content view in focus.

tvOS 13.0+

``` source
@MainActor
var maskedContentView: UIView { get }
```

## Discussion

Use this property to modify the parallax effect applied on the cell and its content. Add any other UI elements to be included on the cell to this view.

This view fills the entire screen.

## See Also

### Accessing Cell Views

var maskedBackgroundView: UIView

The background view that performs the parallax effect.

