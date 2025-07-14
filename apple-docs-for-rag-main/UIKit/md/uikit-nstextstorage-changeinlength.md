

- UIKit
- NSTextStorage
-  changeInLength 

Instance Property

# changeInLength

The difference between the current length of the edited range and its length before editing.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var changeInLength: Int { get }
```

## Discussion

This property reflects difference between the current length of the edited range and its length before editing began—that is, before the first call to the beginEditing() method or a single call to theedited(_:range:changeInLength:) method. This difference is accumulated with each call to the edited(_:range:changeInLength:) method, until the changes are finally processed.

The text storage object’s delegate and layout managers can use this information to determine the nature of edits in their respective notification methods.

## See Also

### Determining the nature of changes

var editedMask: NSTextStorage.EditActions

A mask that describes the kinds of edits pending for the text storage object.

var editedRange: NSRange

The range of text that contains changes.

