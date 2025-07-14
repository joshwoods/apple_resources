

- UIKit
- UIViewControllerPreviewing
-  sourceView Deprecated

Instance Property

# sourceView

A source view, in a previewing view controller’s view hierarchy, responds to a 3D Touch by the user.

iOS 9.0–13.0DeprecatediPadOS 9.0–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedtvOS 9.0–13.0Deprecated

``` source
@MainActor
var sourceView: UIView { get }
```

**Required**

## Discussion

Set the value of this property when you register a view controller to participate in 3D Touch. Do this in the view controller’s registerForPreviewing(with:sourceView:) method.

When the user begins to press on the source view, the system blurs the surrounding area to let the user know that a preview (peek) is available. At this time, the system calls your previewingContext(_:viewControllerForLocation:) method to let you prepare the presentation of a preview. If the user presses more deeply, the system presents the preview defined in your delegate method.

If the user presses deeper on the preview, the system navigates to the view you’ve specified in your previewingContext(_:commit:) method. The commit view then fills the bounds of the app’s window.

## See Also

### Related Documentation

var sourceRect: CGRect

The rectangle, in the source view’s coordinate system, that responds to a 3D Touch by a user and remains visually sharp while surrounding content blurs.

**Required**

Deprecated

### Accessing properties of a 3D Touch previewing view controller

var delegate: any UIViewControllerPreviewingDelegate

The previewing view controller’s delegate for managing preview (peek) and commit (pop) view controllers.

**Required**

Deprecated

