

- WebKit
- WebView
-  setSelectedDOMRange(\_:affinity:) 

Instance Method

# setSelectedDOMRange(\_:affinity:)

Selects a range of nodes.

macOS

``` source
@MainActor
func setSelectedDOMRange(
    _ range: DOMRange!,
    affinity selectionAffinity: NSSelectionAffinity
)
```

## Parameters 

`range`  

The range of nodes to select. If `range` is `nil`, the current selection is cleared. This method raises a `DOMRangeExcepton` if the range has been detached or refers to nodes not displayed by the receiver.

`selectionAffinity`  

See the selectionAffinity property for information on selection affinity.

## See Also

### Related Documentation

func editableDOMRange(for: NSPoint) -> DOMRange!

Returns the editable DOM object located at a given point.

### Selecting Content in the Document

var selectedDOMRange: DOMRange!

The range of the current selection.

var selectionAffinity: NSSelectionAffinity

The current selection affinity.

