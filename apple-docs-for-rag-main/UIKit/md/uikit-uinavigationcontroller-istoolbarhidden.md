

- UIKit
- UINavigationController
-  isToolbarHidden 

Instance Property

# isToolbarHidden

A Boolean indicating whether the navigation controller’s built-in toolbar is visible.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isToolbarHidden: Bool { get set }
```

## Discussion

If this property is set to true, the toolbar is not visible. The default value of this property is true.

## See Also

### Configuring custom toolbars

var toolbar: UIToolbar!

The custom toolbar associated with the navigation controller.

func setToolbarHidden(Bool, animated: Bool)

Changes the visibility of the navigation controller’s built-in toolbar.

class let hideShowBarDuration: CGFloat

A variable that specifies the duration when animating the navigation bar.

