

- Foundation
- NSMutableAttributedString
-  insert(\_:at:) 

Instance Method

# insert(\_:at:)

Inserts the characters and attributes of the given attributed string into the receiver at the given index.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func insert(
    _ attrString: NSAttributedString,
    at loc: Int
)
```

## Parameters 

`attrString`  

The string whose characters and attributes are inserted.

`loc`  

The index at which the characters and attributes are inserted.

## Discussion

The new characters and attributes begin at the given index and the existing characters and attributes from the index to the end of the receiver are shifted by the length of the attributed string. Raises an rangeException if `loc` lies beyond the end of the receiver’s characters.

## See Also

### Changing Characters and Attributes

func append(NSAttributedString)

Adds the characters and attributes of a given attributed string to the end of the receiver.

func replaceCharacters(in: NSRange, with: NSAttributedString)

Replaces the characters and attributes in a given range with the characters and attributes of the given attributed string.

func setAttributedString(NSAttributedString)

Replaces the receiver’s entire contents with the characters and attributes of the given attributed string.

