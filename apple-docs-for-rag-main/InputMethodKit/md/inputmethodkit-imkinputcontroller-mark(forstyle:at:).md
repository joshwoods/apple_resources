

- InputMethodKit
- IMKInputController
-  mark(forStyle:at:) 

Instance Method

# mark(forStyle:at:)

Returns a dictionary of text attributes that can mark a range of an attributed string to send to a client.

macOS 10.5+

``` source
func mark(
    forStyle style: Int,
    at range: NSRange
) -> [AnyHashable : Any]!
```

## Parameters 

`style`  

A style, which should be one of the following values: kTSMHiliteSelectedRawText, kTSMHiliteConvertedText, or kTSMHiliteSelectedConvertedText. See the `AERegistry.h` header file for the definition of these values.

`range`  

The range (that is, a clause) to mark.

## Return Value

The dictionary of text attributes.

## Discussion

This utility function can be called by input methods to mark each range (i.e. clause ) of marked text. T

The default implementation first calls the method compositionAttributes(at:) to obtain the additional attributes that an input method wants to include, such as font or glyph information. Then, it adds the appropriate underline and underline color information to the attributes dictionary for the style parameter. Finally it adds the style value as the dictionary value. The key for the style value is markedClauseSegment.

## See Also

### Working with Ranges

func compositionAttributes(at: NSRange) -> NSMutableDictionary!

Returns a dictionary of text attributes.

func selectionRange() -> NSRange

Returns where the range of the selection that should be placed inside marked text.

func replacementRange() -> NSRange

Returns the range in the client document that the text should replace.

