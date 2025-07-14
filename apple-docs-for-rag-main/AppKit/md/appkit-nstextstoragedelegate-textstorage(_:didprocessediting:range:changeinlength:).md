

- AppKit
- NSTextStorageDelegate
-  textStorage(\_:didProcessEditing:range:changeInLength:) 

Instance Method

# textStorage(\_:didProcessEditing:range:changeInLength:)

The method the framework calls when a text storage object has finished processing edits.

macOS 10.11+

``` source
optional func textStorage(
    _ textStorage: NSTextStorage,
    didProcessEditing editedMask: NSTextStorageEditActions,
    range editedRange: NSRange,
    changeInLength delta: Int
)
```

## Parameters 

`textStorage`  

The text storage object processing edits.

`editedMask`  

The types of edits done: editedAttributes, editedCharacters, or both.

`editedRange`  

The range in the original string (before the edit).

`delta`  

The length delta for the editing changes.

## Discussion

Sent inside processEditing() right before notifying layout managers. Delegates can change the attributes.

The delegate can verify the final state of the text storage object; it can’t change the text storage object’s characters without leaving it in an inconsistent state, but if necessary it can change attributes. Note that even in this case it’s possible to put a text storage object into an inconsistent state—for example, by changing the font of a range to one that doesn’t support the characters in that range, such as using a Latin font for Kanji text.

## See Also

### Processing edit actions

func textStorage(NSTextStorage, willProcessEditing: NSTextStorageEditActions, range: NSRange, changeInLength: Int)

The method the framework calls when a text storage object is about to process edits.

