

- UIKit
- UIStatusBarManager
-  statusBarStyle 

Instance Property

# statusBarStyle

The current appearance of the status bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var statusBarStyle: UIStatusBarStyle { get }
```

## Discussion

To customize the status bar’s style for each of your view controllers, override their preferredStatusBarStyle property.

## See Also

### Getting the status bar configuration

var isStatusBarHidden: Bool

A Boolean value that indicates whether the status bar is currently hidden.

