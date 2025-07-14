

- AppKit
- NSTextInputClient
-  attributedString() 

Instance Method

# attributedString()

Returns an attributed string representing the receiver’s text storage.

macOS 10.0+

``` source
optional func attributedString() -> NSAttributedString
```

## Return Value

The attributed string of the receiver’s text storage.

## Discussion

Implementation of this method is optional. A class adopting the `NSTextInputClient` protocol can implement this interface if it can be done efficiently to enable callers of this interface to access arbitrary portions of the receiver’s content more efficiently.

## See Also

### Storing text

func attributedSubstring(forProposedRange: NSRange, actualRange: NSRangePointer?) -> NSAttributedString?

Returns an attributed string derived from the given range in the receiver’s text storage.

**Required**

func insertText(Any, replacementRange: NSRange)

Inserts the given string into the receiver, replacing the specified content.

**Required**

