

- TVUIKit
- TVLockupView
-  contentView 

Instance Property

# contentView

The main view for the lockup.

tvOS 12.0+

``` source
@MainActor
var contentView: UIView { get }
```

## Discussion

Add subviews to the `contentView`. Don’t add views direcly to the lockup view.

## See Also

### Adding subviews

var headerView: TVLockupHeaderFooterView?

A view containing header information.

var footerView: TVLockupHeaderFooterView?

A view containing footer information.

