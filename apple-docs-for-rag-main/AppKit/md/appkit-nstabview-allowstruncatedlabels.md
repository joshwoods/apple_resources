

- AppKit
- NSTabView
-  allowsTruncatedLabels 

Instance Property

# allowsTruncatedLabels

A Boolean value that indicates if the tab view allows truncating for labels that don’t fit on a tab.

macOS

``` source
@MainActor
var allowsTruncatedLabels: Bool { get set }
```

## Discussion

When the value of this property is true, the tab view allows truncating for labels that don’t fit on a tab, otherwise it does not. The default value is true. When truncating is allowed, the tab view inserts an ellipsis, if necessary, to fit a label in the tab.

