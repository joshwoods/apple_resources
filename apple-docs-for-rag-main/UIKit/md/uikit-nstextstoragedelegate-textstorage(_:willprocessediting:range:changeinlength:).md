

- UIKit
- NSTextStorageDelegate
-  textStorage(\_:willProcessEditing:range:changeInLength:) 

Instance Method

# textStorage(\_:willProcessEditing:range:changeInLength:)

The method the framework calls when a text storage object is about to process edits.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
optional func textStorage(
    _ textStorage: NSTextStorage,
    willProcessEditing editedMask: NSTextStorage.EditActions,
    range editedRange: NSRange,
    changeInLength delta: Int
)
```

## Parameters 

`textStorage`  

The text storage object processing edits.

`editedMask`  

The types of edits to do: editedAttributes, editedCharacters, or both.

`editedRange`  

The range in the original string (before the edit).

`delta`  

The length delta for the editing changes.

## Discussion

Sent inside processEditing() right before fixing attributes. Delegates can change the characters or attributes.

The delegate can verify the changed state of the text storage object and make changes to the text storage object’s characters or attributes to enforce whatever constraints it establishes. Programmatic changes don’t cause the object to send this message.

## See Also

### Processing edit actions

func textStorage(NSTextStorage, didProcessEditing: NSTextStorage.EditActions, range: NSRange, changeInLength: Int)

The method the framework calls when a text storage object has finished processing edits.

