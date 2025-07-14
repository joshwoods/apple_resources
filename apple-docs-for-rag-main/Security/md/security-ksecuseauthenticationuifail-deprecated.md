

- Security
-  kSecUseAuthenticationUIFail Deprecated

Global Variable

# kSecUseAuthenticationUIFail

A value that indicates user authentication is disallowed.

iOS 9.0–14.0DeprecatediPadOS 9.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.11–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–7.0Deprecated

``` source
let kSecUseAuthenticationUIFail: CFString
```

Deprecated

Instead of kSecUseAuthenticationUI, use kSecUseAuthenticationContext and set LAContext.interactionNotAllowed property

## Discussion

When you specify this value, if user authentication is needed, the function returns the errSecInteractionNotAllowed error.

