

- UIKit
- UIPrintFormatter
-  requiresMainThread 

Instance Property

# requiresMainThread

A Boolean value that determines whether the system executes the print formatter’s rendering operations on the main thread.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var requiresMainThread: Bool { get }
```

## Discussion

The default value is true, which requires the printing system to execute rendering operations, like drawing and page-count calculation, on the main thread. Override this property to return false if you want the system to execute operations like draw(in:forPageAt:) and pageCount on a background thread.

