

- UIKit
- UIStatusBarManager
-  isStatusBarHidden 

Instance Property

# isStatusBarHidden

A Boolean value that indicates whether the status bar is currently hidden.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var isStatusBarHidden: Bool { get }
```

## Discussion

To customize the status bar’s visibility for each of your view controllers, override your view controller’s prefersStatusBarHidden property.

## See Also

### Getting the status bar configuration

var statusBarStyle: UIStatusBarStyle

The current appearance of the status bar.

