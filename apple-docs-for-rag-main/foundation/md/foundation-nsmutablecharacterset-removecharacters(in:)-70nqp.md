

- Foundation
- NSMutableCharacterSet
-  removeCharacters(in:) 

Instance Method

# removeCharacters(in:)

Removes from the receiver the characters whose Unicode values are in a given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func removeCharacters(in aRange: NSRange)
```

## Parameters 

`aRange`  

The range of characters to remove. `aRange.location` is the value of the first character to remove; `aRange.location + aRange.length – 1` is the value of the last. If `aRange.length` is `0`, this method has no effect.

## See Also

### Adding and Removing Characters

func addCharacters(in: NSRange)

Adds to the receiver the characters whose Unicode values are in a given range.

func addCharacters(in: String)

Adds to the receiver the characters in a given string.

func removeCharacters(in: String)

Removes from the receiver the characters in a given string.

