

- Security
-  kSecUseAuthenticationUI 

Global Variable

# kSecUseAuthenticationUI

A key whose value indicates whether the user is prompted for authentication.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecUseAuthenticationUI: CFString
```

## Discussion

The corresponding value is of type CFString and contains one of the values listed in UI authentication values. The value specifies whether or not the user is prompted for authentication, if needed. A default value of kSecUseAuthenticationUIAllow is assumed when this key is not present.

