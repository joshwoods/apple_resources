

- Security
-  kSecUseAuthenticationUISkip 

Global Variable

# kSecUseAuthenticationUISkip

A value that indicates items requiring user authentication should be skipped.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecUseAuthenticationUISkip: CFString
```

## Discussion

Silently skip any items that require user authentication. Only use this value with the SecItemCopyMatching(_:_:) function.

