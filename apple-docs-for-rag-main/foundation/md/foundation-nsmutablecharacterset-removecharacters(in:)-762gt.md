

- Foundation
- NSMutableCharacterSet
-  removeCharacters(in:) 

Instance Method

# removeCharacters(in:)

Removes from the receiver the characters in a given string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeCharacters(in aString: String)
```

## Parameters 

`aString`  

The characters to remove from the receiver.

## Discussion

This method has no effect if `aString` is empty.

## See Also

### Adding and Removing Characters

func addCharacters(in: NSRange)

Adds to the receiver the characters whose Unicode values are in a given range.

func removeCharacters(in: NSRange)

Removes from the receiver the characters whose Unicode values are in a given range.

func addCharacters(in: String)

Adds to the receiver the characters in a given string.

