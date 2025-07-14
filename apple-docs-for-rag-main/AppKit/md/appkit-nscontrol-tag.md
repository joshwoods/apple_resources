

- AppKit
- NSControl
-  tag 

Instance Property

# tag

The tag identifying the receiver (not the tag of the receiver’s cell).

macOS

``` source
@MainActor
var tag: Int { get set }
```

## Discussion

Tags allow you to identify particular controls. Tag values are not used internally; they are only changed when you set this property. You typically set tag values in Interface Builder and use them at runtime in your application. When you set the tag of a control with a single cell in Interface Builder, it sets the tags of both the control and the cell to the same value as a convenience.

## See Also

### Related Documentation

func selectedTag() -> Int

Returns the tag of the receiver’s selected cell.

