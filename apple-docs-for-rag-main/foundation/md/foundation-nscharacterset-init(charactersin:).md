

- Foundation
- NSCharacterSet
-  init(charactersIn:) 

Initializer

# init(charactersIn:)

Returns a character set containing the characters in a given string.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(charactersIn aString: String)
```

## Parameters 

`aString`  

A string containing characters for the new character set.

## Return Value

A character set containing the characters in `aString`. Returns an empty character set if `aString` is empty.

## See Also

### Creating a Custom Character Set

init(coder: NSCoder)

init(range: NSRange)

Returns a character set containing characters with Unicode values in a given range.

NSOpenStepUnicodeReservedBase

Specifies lower bound for a Unicode character range reserved for Apple’s corporate use.

