

- UIKit
- UIViewControllerPreviewing
-  delegate Deprecated

Instance Property

# delegate

The previewing view controller’s delegate for managing preview (peek) and commit (pop) view controllers.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
var delegate: any UIViewControllerPreviewingDelegate { get }
```

**Required**

## Discussion

Set a previewing view controller’s 3D Touch delegate when you register the view controller by calling its registerForPreviewing(with:sourceView:) method.

For information on the methods the delegate can implement, read UIViewControllerPreviewingDelegate.

## See Also

### Accessing properties of a 3D Touch previewing view controller

var sourceView: UIView

A source view, in a previewing view controller’s view hierarchy, responds to a 3D Touch by the user.

**Required**

Deprecated

