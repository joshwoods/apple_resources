

- Security
-  kSecUseNoAuthenticationUI Deprecated

Global Variable

# kSecUseNoAuthenticationUI

A key whose value is a Boolean indicating whether to disallow UI authentication.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.10–10.11DeprecatedtvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
let kSecUseNoAuthenticationUI: CFString
```

Deprecated

Use the key kSecUseAuthenticationUI with value kSecUseAuthenticationUIFail instead.

## Discussion

The corresponding value is of type CFBoolean. If provided with a value of kCFBooleanTrue, the error errSecInteractionNotAllowed is returned when the item is attempting to authenticate with UI.

