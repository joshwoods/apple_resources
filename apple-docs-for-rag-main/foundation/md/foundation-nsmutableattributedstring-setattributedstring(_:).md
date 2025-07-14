

- Foundation
- NSMutableAttributedString
-  setAttributedString(\_:) 

Instance Method

# setAttributedString(\_:)

Replaces the receiver’s entire contents with the characters and attributes of the given attributed string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setAttributedString(_ attrString: NSAttributedString)
```

## Parameters 

`attrString`  

The attributed string whose characters and attributes replace those in the receiver.

## See Also

### Changing Characters and Attributes

func append(NSAttributedString)

Adds the characters and attributes of a given attributed string to the end of the receiver.

func insert(NSAttributedString, at: Int)

Inserts the characters and attributes of the given attributed string into the receiver at the given index.

func replaceCharacters(in: NSRange, with: NSAttributedString)

Replaces the characters and attributes in a given range with the characters and attributes of the given attributed string.

