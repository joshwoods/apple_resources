

- AppKit
- NSTextView
-  usesFindBar 

Instance Property

# usesFindBar

A Boolean value that indicates whether to use the find bar for this text view.

macOS 10.7+

``` source
@MainActor
var usesFindBar: Bool { get set }
```

## Discussion

The value of this property is true if the find bar is used for this text view; otherwise false. See NSTextFinder for information about the find bar.

A text view can use either a find panel or a find bar. If usesFindBar is set to true, usesFindPanel is set to false and vice versa.

## See Also

### Related Documentation

var usesFindPanel: Bool

A Boolean value that indicates whether the receiver allows for a find panel.

### Using the Find Bar

var isIncrementalSearchingEnabled: Bool

A Boolean value that indicates whether incremental searching is enabled.

