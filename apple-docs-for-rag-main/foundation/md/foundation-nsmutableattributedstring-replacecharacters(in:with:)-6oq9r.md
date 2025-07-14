

- Foundation
- NSMutableAttributedString
-  replaceCharacters(in:with:) 

Instance Method

# replaceCharacters(in:with:)

Replaces the characters in the given range with the characters of the given string.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func replaceCharacters(
    in range: NSRange,
    with str: String
)
```

## Parameters 

`range`  

A range specifying the characters to replace.

`str`  

A string specifying the characters to replace those in `range`.

## Discussion

The new characters inherit the attributes of the first replaced character from `range`. Where the length of `range` is 0, the new characters inherit the attributes of the character preceding `range` if it has any, otherwise of the character following `range`.

Raises an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

## See Also

### Changing Characters

func deleteCharacters(in: NSRange)

Deletes the characters in the given range along with their associated attributes.

