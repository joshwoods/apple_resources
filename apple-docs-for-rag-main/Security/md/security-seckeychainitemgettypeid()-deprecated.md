

- Security
-  SecKeychainItemGetTypeID() Deprecated

Function

# SecKeychainItemGetTypeID()

Returns the unique identifier of the opaque type to which a keychain item object belongs.

macOS 10.2–10.10Deprecated

``` source
func SecKeychainItemGetTypeID() -> CFTypeID
```

Deprecated

SecKeychain is deprecated

## Return Value

A value that identifies the opaque type of a SecKeychainItem object.

## Discussion

This function returns a value that uniquely identifies the opaque type of a SecKeychainItem object. You can compare this value to the CFTypeID identifier obtained by calling the CFGetTypeID(_:) function on a specific object. These values might change from release to release or platform to platform.

