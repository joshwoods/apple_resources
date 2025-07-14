

- Foundation
- NSAttributedString
-  rulerAttributes(in:) 

Instance Method

# rulerAttributes(in:)

Returns the ruler (paragraph) attributes in effect for the characters within the specified range.

macOS 10.0+

``` source
func rulerAttributes(in range: NSRange) -> [NSAttributedString.Key : Any]
```

## Parameters 

`range`  

The range.

## Return Value

A dictionary containing the ruler attributes in the range.

## Discussion

The only ruler attribute currently defined is that named by paragraphStyle. Use this method to obtain attributes that are to be copied or pasted with “copy ruler” operations.

Raises an rangeException if any part of `aRange` lies beyond the end of the receiver’s characters.

## See Also

### Getting font attribute information

func fontAttributes(in: NSRange) -> [NSAttributedString.Key : Any]

Returns the font attributes in effect for the character at the specified location.

