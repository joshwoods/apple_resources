

- Foundation
- NSMutableCharacterSet
-  addCharacters(in:) 

Instance Method

# addCharacters(in:)

Adds to the receiver the characters whose Unicode values are in a given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addCharacters(in aRange: NSRange)
```

## Parameters 

`aRange`  

The range of characters to add. `aRange.location` is the value of the first character to add; `aRange.location + aRange.length – 1` is the value of the last. If `aRange.length` is `0`, this method has no effect.

## Discussion

This code excerpt adds to a character set the lowercase English alphabetic characters:

```
NSMutableCharacterSet *aCharacterSet = [[NSMutableCharacterSet alloc] init];
NSRange lcEnglishRange;

lcEnglishRange.location = (unsigned int)'a';
lcEnglishRange.length = 26;
[aCharacterSet addCharactersInRange:lcEnglishRange];
```

## See Also

### Related Documentation

String Programming Guide

### Adding and Removing Characters

func removeCharacters(in: NSRange)

Removes from the receiver the characters whose Unicode values are in a given range.

func addCharacters(in: String)

Adds to the receiver the characters in a given string.

func removeCharacters(in: String)

Removes from the receiver the characters in a given string.

