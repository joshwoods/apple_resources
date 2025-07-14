

- Security
-  kSecMatchCaseInsensitive 

Global Variable

# kSecMatchCaseInsensitive

A key whose value is a Boolean indicating whether case-insensitive matching is performed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecMatchCaseInsensitive: CFString
```

## Discussion

The corresponding value is of type CFBoolean. If this value is kCFBooleanFalse, or if this attribute is not provided, then case-sensitive string matching is performed.

