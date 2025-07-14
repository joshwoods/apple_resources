

- Security
-  kSecAttrAccessibleWhenUnlockedThisDeviceOnly 

Global Variable

# kSecAttrAccessibleWhenUnlockedThisDeviceOnly

The data in the keychain item can be accessed only while the device is unlocked by the user.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let kSecAttrAccessibleWhenUnlockedThisDeviceOnly: CFString
```

## Mentioned in 

Protecting keys with the Secure Enclave

## Discussion

This is recommended for items that need to be accessible only while the application is in the foreground. Items with this attribute *do not* migrate to a new device. Thus, after restoring from a backup of a different device, these items will not be present.

