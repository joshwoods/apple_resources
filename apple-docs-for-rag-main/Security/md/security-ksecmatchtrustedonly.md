

- Security
-  kSecMatchTrustedOnly 

Global Variable

# kSecMatchTrustedOnly

A key whose value is a Boolean indicating whether untrusted certificates should be returned.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecMatchTrustedOnly: CFString
```

## Discussion

The corresponding value is of type CFBoolean. If this attribute is provided with a value of kCFBooleanTrue, only certificates that can be verified back to a trusted anchor are returned. If this value is kCFBooleanFalse or the attribute is not provided, then both trusted and untrusted certificates may be returned.

