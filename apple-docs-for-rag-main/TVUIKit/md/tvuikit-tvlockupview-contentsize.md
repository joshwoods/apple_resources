

- TVUIKit
- TVLockupView
-  contentSize 

Instance Property

# contentSize

The size of the content view.

tvOS 12.0+

``` source
@MainActor
var contentSize: CGSize { get set }
```

## Discussion

Use this property to explicitly set the size of the content view. If frame is explicitly set, it takes precedence over `contentSize`.

## See Also

### Setting view size

var contentViewInsets: NSDirectionalEdgeInsets

The spacing between the content view and its peer and containing views.

var focusSizeIncrease: NSDirectionalEdgeInsets

The inset or outset values specifying your content’s size increase when in focus.

