

- Security
-  kSecUseUserIndependentKeychain 

Global Variable

# kSecUseUserIndependentKeychain

A key with a value that indicates whether to store the data in a keychain available to anyone who uses the device.

tvOS 16.0+

``` source
let kSecUseUserIndependentKeychain: CFString
```

## Discussion

The corresponding value is of type CFBoolean. A value of kCFBooleanTrue stores the item in a shared keychain that your app can access even when a different user is active. A value of kCFBooleanFalse or omitting this key-value pair stores the item in the current user’s keychain.

To view a sample code project that uses this key to streamline experiences like family media accounts, see Mapping Apple TV users to app profiles.

