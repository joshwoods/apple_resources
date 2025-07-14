

- AppKit
- NSCell
-  representedObject 

Instance Property

# representedObject

The object represented by the cell.

macOS

``` source
@MainActor
var representedObject: Any? { get set }
```

## Discussion

Use this property to link the cell an appropriate object. For example, in a pop-up list of color names, the represented object of each cell could be the appropriate NSColor object.

### Special Considerations

When you copy an `NSCell` object, the value of this property is set to `nil` in the copy.

## See Also

### Related Documentation

var objectValue: Any?

The cell’s value as an Objective-C object.

