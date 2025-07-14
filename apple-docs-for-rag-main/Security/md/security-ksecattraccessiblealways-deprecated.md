

- Security
-  kSecAttrAccessibleAlways Deprecated

Global Variable

# kSecAttrAccessibleAlways

The data in the keychain item can always be accessed regardless of whether the device is locked.

iOS 4.0–12.0DeprecatediPadOS 4.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.14DeprecatedtvOS 9.0–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–5.0Deprecated

``` source
let kSecAttrAccessibleAlways: CFString
```

Deprecated

Use an accessibility level that provides some user protection, such as kSecAttrAccessibleAfterFirstUnlock

## Discussion

This is not recommended for application use. Items with this attribute migrate to a new device when using encrypted backups.

