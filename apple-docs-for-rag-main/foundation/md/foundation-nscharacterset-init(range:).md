

- Foundation
- NSCharacterSet
-  init(range:) 

Initializer

# init(range:)

Returns a character set containing characters with Unicode values in a given range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(range aRange: NSRange)
```

## Parameters 

`aRange`  

A range of Unicode values. `aRange.location` is the value of the first character to return; `aRange.location + aRange.length – 1` is the value of the last.

## Return Value

A character set containing characters whose Unicode values are given by `aRange`. If `aRange.length` is `0`, returns an empty character set.

## Discussion

This code excerpt creates a character set object containing the lowercase English alphabetic characters:

```
NSRange lcEnglishRange;
NSCharacterSet *lcEnglishLetters;

lcEnglishRange.location = (unsigned int)'a';
lcEnglishRange.length = 26;
lcEnglishLetters = [NSCharacterSet characterSetWithRange:lcEnglishRange];
```

## See Also

### Creating a Custom Character Set

init(coder: NSCoder)

init(charactersIn: String)

Returns a character set containing the characters in a given string.

NSOpenStepUnicodeReservedBase

Specifies lower bound for a Unicode character range reserved for Apple’s corporate use.

