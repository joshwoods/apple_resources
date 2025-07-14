

- Foundation
- NSMutableCharacterSet
-  addCharacters(in:) 

Instance Method

# addCharacters(in:)

Adds to the receiver the characters in a given string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addCharacters(in aString: String)
```

## Parameters 

`aString`  

The characters to add to the receiver.

## Discussion

This method has no effect if `aString` is empty.

## See Also

### Adding and Removing Characters

func addCharacters(in: NSRange)

Adds to the receiver the characters whose Unicode values are in a given range.

func removeCharacters(in: NSRange)

Removes from the receiver the characters whose Unicode values are in a given range.

func removeCharacters(in: String)

Removes from the receiver the characters in a given string.

