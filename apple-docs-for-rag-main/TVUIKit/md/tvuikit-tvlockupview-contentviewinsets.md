

- TVUIKit
- TVLockupView
-  contentViewInsets 

Instance Property

# contentViewInsets

The spacing between the content view and its peer and containing views.

tvOS 12.0+

``` source
@MainActor
var contentViewInsets: NSDirectionalEdgeInsets { get set }
```

## Discussion

Use negative values for positive spacing. The top and bottom values represent the spacing between the content view and the header and footer views, respectively. The leading and trailing values represent the spacing between the content view and the lockup view. The default value is NSDirectionalEdgeInsetsZero.

## See Also

### Setting view size

var contentSize: CGSize

The size of the content view.

var focusSizeIncrease: NSDirectionalEdgeInsets

The inset or outset values specifying your content’s size increase when in focus.

