

- Security
- SecKeychainCallbackInfo
-  init(version:item:keychain:pid:) 

Initializer

# init(version:item:keychain:pid:)

Creates a new keychain callback information structure.

macOS 10.0+

``` source
init(
    version: UInt32,
    item: Unmanaged,
    keychain: Unmanaged,
    pid: pid_t
)
```

