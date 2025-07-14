

- WebKit
- WKSnapshotConfiguration
-  afterScreenUpdates 

Instance Property

# afterScreenUpdates

A Boolean value that indicates whether to take the snapshot after incorporating any pending screen updates.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+visionOS 1.0+

``` source
@MainActor
var afterScreenUpdates: Bool { get set }
```

## Discussion

The default value of this property is true, which causes the web view to incorporate any recent changes to the view’s content and then generate the snapshot. If you change the value to false, the web view takes the snapshot immediately, and before incorporating any new changes.

