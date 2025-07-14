

- UIKit
- UIStatusBarManager
-  statusBarFrame 

Instance Property

# statusBarFrame

The frame rectangle of the status bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var statusBarFrame: CGRect { get }
```

## Discussion

The frame rectangle is in the coordinate space of the associated UIWindowScene object. If the status bar is hidden, the value of this property is CGRectZero.

