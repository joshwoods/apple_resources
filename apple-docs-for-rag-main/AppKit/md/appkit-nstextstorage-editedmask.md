

- AppKit
- NSTextStorage
-  editedMask 

Instance Property

# editedMask

A mask that describes the kinds of edits pending for the text storage object.

macOS 10.0+

``` source
var editedMask: NSTextStorageEditActions { get }
```

## Discussion

This property indicates pending changes for attributes, characters, or both. Use the C bitwise AND operator to test the value against the editedAttributes or editedCharacters constants; testing for equality fails if you add additional mask flags later. The text storage object’s associated delegate and layout managers can use this information to determine the nature of edits in their respective notification methods.

## See Also

### Determining the nature of changes

var editedRange: NSRange

The range of text that contains changes.

var changeInLength: Int

The difference between the current length of the edited range and its length before editing.

