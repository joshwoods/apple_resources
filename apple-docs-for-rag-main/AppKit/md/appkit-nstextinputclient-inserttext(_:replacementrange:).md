

- AppKit
- NSTextInputClient
-  insertText(\_:replacementRange:) 

Instance Method

# insertText(\_:replacementRange:)

Inserts the given string into the receiver, replacing the specified content.

macOS

``` source
func insertText(
    _ string: Any,
    replacementRange: NSRange
)
```

**Required**

## Parameters 

`string`  

The text to insert, either an `NSString` or `NSAttributedString` instance.

`replacementRange`  

The range of content to replace in the receiver’s text storage.

## Mentioned in 

Supporting Writing Tools via the pasteboard

## Discussion

This method is the entry point for inserting text typed by the user and is generally not suitable for other purposes. Programmatic modification of the text is best done by operating on the text storage directly. Because this method pertains to the actions of the user, the text view must be editable for the insertion to work.

## See Also

### Storing text

func attributedString() -> NSAttributedString

Returns an attributed string representing the receiver’s text storage.

func attributedSubstring(forProposedRange: NSRange, actualRange: NSRangePointer?) -> NSAttributedString?

Returns an attributed string derived from the given range in the receiver’s text storage.

**Required**

