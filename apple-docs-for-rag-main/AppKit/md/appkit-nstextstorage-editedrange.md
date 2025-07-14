

- AppKit
- NSTextStorage
-  editedRange 

Instance Property

# editedRange

The range of text that contains changes.

macOS 10.0+

``` source
var editedRange: NSRange { get }
```

## Discussion

The specified range can reflect changes to characters or attributes. The text storage object’s delegate and layout managers can use this information to determine the nature of edits in their respective notification methods.

## See Also

### Determining the nature of changes

var editedMask: NSTextStorageEditActions

A mask that describes the kinds of edits pending for the text storage object.

var changeInLength: Int

The difference between the current length of the edited range and its length before editing.

