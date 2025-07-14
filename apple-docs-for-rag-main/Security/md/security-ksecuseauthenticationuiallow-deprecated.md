

- Security
-  kSecUseAuthenticationUIAllow Deprecated

Global Variable

# kSecUseAuthenticationUIAllow

A value that indicates user authentication is allowed.

iOS 9.0–14.0DeprecatediPadOS 9.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.11–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–7.0Deprecated

``` source
let kSecUseAuthenticationUIAllow: CFString
```

Deprecated

Instead of kSecUseAuthenticationUI, use kSecUseAuthenticationContext and set LAContext.interactionNotAllowed property

## Discussion

The user may be prompted for authentication. This is the default value.

