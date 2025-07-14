

- InputMethodKit
- IMKInputController
-  replacementRange() 

Instance Method

# replacementRange()

Returns the range in the client document that the text should replace.

macOS 10.5+

``` source
func replacementRange() -> NSRange
```

## Return Value

The range to replace.

## Discussion

This method is called by updateComposition() to obtain the range in the client document where marked text should be placed. The default implementation returns an `NSRange` object whose location and length are `NSNotFound`. That indicates that the marked text should be placed at the current insertion point. Input methods that insert marked text somewhere other than at the current insertion point should override this method.

An example of an input method that might override this method would be one replaces words with synonyms. That input method would watch for certain words and when it detects such a word it would replaced the word by marked text that was a synonym of the word.

## See Also

### Working with Ranges

func compositionAttributes(at: NSRange) -> NSMutableDictionary!

Returns a dictionary of text attributes.

func selectionRange() -> NSRange

Returns where the range of the selection that should be placed inside marked text.

func mark(forStyle: Int, at: NSRange) -> [AnyHashable : Any]!

Returns a dictionary of text attributes that can mark a range of an attributed string to send to a client.

