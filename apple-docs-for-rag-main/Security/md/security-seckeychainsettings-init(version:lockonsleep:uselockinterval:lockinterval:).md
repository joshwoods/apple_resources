

- Security
- SecKeychainSettings
-  init(version:lockOnSleep:useLockInterval:lockInterval:) 

Initializer

# init(version:lockOnSleep:useLockInterval:lockInterval:)

Initializes a keychain settings structures with the given values.

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    version: UInt32,
    lockOnSleep: DarwinBoolean,
    useLockInterval: DarwinBoolean,
    lockInterval: UInt32
)
```

## Parameters 

`version`  

The keychain version. Use SEC_KEYCHAIN_SETTINGS_VERS1.

`lockOnSleep`  

A Boolean indicating whether the keychain locks when the system enters sleep mode.

`useLockInterval`  

A Boolean indicating whether the keychain locks after an time period elapses, as given by lockInterval.

`lockInterval`  

The number of seconds after which the keychain should lock if useLockInterval is true.

