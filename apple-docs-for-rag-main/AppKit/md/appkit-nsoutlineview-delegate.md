

- AppKit
- NSOutlineView
-  delegate 

Instance Property

# delegate

The outline view’s delegate.

macOS

``` source
@MainActor
weak var delegate: (any NSOutlineViewDelegate)? { get set }
```

## Discussion

The delegate must conform to the NSOutlineViewDelegate protocol. Note that in versions of macOS prior to v10.12, the table view did not retain the delegate in a managed memory environment.

