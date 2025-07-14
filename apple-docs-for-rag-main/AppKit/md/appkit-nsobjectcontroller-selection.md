

- AppKit
- NSObjectController
-  selection 

Instance Property

# selection

A proxy object representing the receiver’s selection.

macOS

``` source
var selection: Any { get }
```

## Discussion

This object is fully key-value coding compliant, but note that it is a proxy and so does not provide the full range of functionality that might be available in the source object.

## See Also

### Obtaining selections

var selectedObjects: [Any]

An array of all objects to be affected by editing.

