

- Security
-  kSecMatchWidthInsensitive 

Global Variable

# kSecMatchWidthInsensitive

A key whose value is a Boolean indicating whether width-insensitive matching is performed.

macOS 10.7+

``` source
let kSecMatchWidthInsensitive: CFString
```

## Discussion

The corresponding value is of type CFBoolean. If this value is kCFBooleanFalse, or if this attribute is not provided, then width-sensitive string matching is performed (for example, the ASCII character `a` does not match the UTF-8 full-width letter `a` (`U+FF41`).

