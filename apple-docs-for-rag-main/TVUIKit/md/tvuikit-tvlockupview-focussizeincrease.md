

- TVUIKit
- TVLockupView
-  focusSizeIncrease 

Instance Property

# focusSizeIncrease

The inset or outset values specifying your content’s size increase when in focus.

tvOS 12.0+

``` source
@MainActor
var focusSizeIncrease: NSDirectionalEdgeInsets { get set }
```

## Discussion

Use negative values for a size increase. The values contribute to the lockup view’s intrinsic content size and guide layout update when focus state changes.

## See Also

### Setting view size

var contentSize: CGSize

The size of the content view.

var contentViewInsets: NSDirectionalEdgeInsets

The spacing between the content view and its peer and containing views.

