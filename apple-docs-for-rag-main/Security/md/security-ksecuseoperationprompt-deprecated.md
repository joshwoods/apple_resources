

- Security
-  kSecUseOperationPrompt Deprecated

Global Variable

# kSecUseOperationPrompt

A key whose value is an operation prompt.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–7.0Deprecated

``` source
let kSecUseOperationPrompt: CFString
```

Deprecated

Use kSecUseAuthenticationContext and set LAContext.localizedReason property

## Discussion

The corresponding value is of type CFString and represents a string describing the operation for which the app is attempting to authenticate. When performing user authentication, the system includes the string in the user prompt. The app is responsible for text localization.

