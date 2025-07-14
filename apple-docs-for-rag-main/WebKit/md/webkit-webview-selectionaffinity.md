

- WebKit
- WebView
-  selectionAffinity 

Instance Property

# selectionAffinity

The current selection affinity.

macOS

``` source
@MainActor
var selectionAffinity: NSSelectionAffinity { get }
```

## Discussion

For example, if text wraps across line boundaries, the value of this property indicates whether or not the insertion point appears after the last charactrer of the first line or before the first character of the following line.

## See Also

### Selecting Content in the Document

var selectedDOMRange: DOMRange!

The range of the current selection.

func setSelectedDOMRange(DOMRange!, affinity: NSSelectionAffinity)

Selects a range of nodes.

