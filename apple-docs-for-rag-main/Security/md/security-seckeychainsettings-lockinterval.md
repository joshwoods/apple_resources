

- Security
- SecKeychainSettings
-  lockInterval 

Instance Property

# lockInterval

The number of seconds to wait before the keychain locks.

Mac Catalyst 13.0+macOS 10.0+

``` source
var lockInterval: UInt32
```

## Discussion

If you set useLockInterval to false, set lockInterval to `INT_MAX` to indicate that the keychain never locks.

