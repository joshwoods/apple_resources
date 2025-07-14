

- WebKit
- WebView
-  selectedDOMRange 

Instance Property

# selectedDOMRange

The range of the current selection.

macOS

``` source
@MainActor
var selectedDOMRange: DOMRange! { get }
```

## Discussion

`nil` if nothing is selected.

## See Also

### Related Documentation

func editableDOMRange(for: NSPoint) -> DOMRange!

Returns the editable DOM object located at a given point.

### Selecting Content in the Document

func setSelectedDOMRange(DOMRange!, affinity: NSSelectionAffinity)

Selects a range of nodes.

var selectionAffinity: NSSelectionAffinity

The current selection affinity.

