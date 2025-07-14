

- AppKit
- NSCell
-  keyEquivalent 

Instance Property

# keyEquivalent

The key equivalent associated with clicking the cell.

macOS

``` source
@MainActor
var keyEquivalent: String { get }
```

## Discussion

Subclasses can override this property and return a string with a valid character for the key equivalent. The default implementation of this property returns an empty string.

