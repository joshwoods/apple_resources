

- Foundation
- NSAttributedString
-  fontAttributes(in:) 

Instance Method

# fontAttributes(in:)

Returns the font attributes in effect for the character at the specified location.

macOS 10.0+

``` source
func fontAttributes(in range: NSRange) -> [NSAttributedString.Key : Any]
```

## Parameters 

`range`  

The range.

## Return Value

A dictionary containing the font attributes for the range.

## Discussion

The dictionary attributes are all those listed in `Character Attributes`, except link, paragraphStyle, and attachment.

Use this method to obtain font attributes that are to be copied or pasted with “copy font” operations.

Raises an `NSRangeException` if any part of `aRange` lies beyond the end of the receiver’s characters.

## See Also

### Getting font attribute information

func rulerAttributes(in: NSRange) -> [NSAttributedString.Key : Any]

Returns the ruler (paragraph) attributes in effect for the characters within the specified range.

