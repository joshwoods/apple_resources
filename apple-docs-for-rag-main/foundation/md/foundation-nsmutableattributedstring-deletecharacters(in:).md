

- Foundation
- NSMutableAttributedString
-  deleteCharacters(in:) 

Instance Method

# deleteCharacters(in:)

Deletes the characters in the given range along with their associated attributes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func deleteCharacters(in range: NSRange)
```

## Parameters 

`range`  

A range specifying the characters to delete.

## Discussion

Raises an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

## See Also

### Related Documentation

func replaceCharacters(in: NSRange, with: NSAttributedString)

Replaces the characters and attributes in a given range with the characters and attributes of the given attributed string.

### Changing Characters

func replaceCharacters(in: NSRange, with: String)

Replaces the characters in the given range with the characters of the given string.

