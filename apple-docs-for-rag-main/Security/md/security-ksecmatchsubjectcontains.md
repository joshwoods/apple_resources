

- Security
-  kSecMatchSubjectContains 

Global Variable

# kSecMatchSubjectContains

A key whose value is a string to look for in a certificate or identity’s subject.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecMatchSubjectContains: CFString
```

## Discussion

The corresponding value is of type CFString. If provided, returned certificates or identities are limited to those whose subject contains this string.

