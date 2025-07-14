

- Security
-  kSecAttrAccessible 

Global Variable

# kSecAttrAccessible

A key with a value that indicates when the keychain item is accessible.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrAccessible: CFString
```

## Mentioned in 

Restricting keychain item accessibility

## Discussion

The corresponding value, one of those found in Accessibility Values, indicates when your app needs access to the data in a keychain item. Choose the most restrictive option that meets your app’s needs so that the system can protect that item to the greatest extent possible. For more information, see Restricting keychain item accessibility.

Important

You can use this attribute for macOS keychain items only if you also set a value of `true` for the kSecUseDataProtectionKeychain key, the kSecAttrSynchronizable key, or both. For any item marked as synchronizable, the value for the kSecAttrAccessible key may only be one whose name does not end with `ThisDeviceOnly`, as those cannot sync to another device.

Note

The app *must* provide the contents of the keychain item (kSecValueData) when changing this attribute in iOS 4 and earlier.

