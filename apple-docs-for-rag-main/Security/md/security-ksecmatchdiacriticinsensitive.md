

- Security
-  kSecMatchDiacriticInsensitive 

Global Variable

# kSecMatchDiacriticInsensitive

A key whose value is a Boolean indicating whether diacritic-insensitive matching is performed.

macOS 10.7+

``` source
let kSecMatchDiacriticInsensitive: CFString
```

## Discussion

The corresponding value is of type CFBoolean. If this value is kCFBooleanFalse, or if this attribute is not provided, then diacritic-sensitive string matching is performed.

