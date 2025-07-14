

- Security
- SecKeychainEventMask
-  passwordChangedEventMask 

Type Property

# passwordChangedEventMask

If the bit specified by this mask is set, your callback function is invoked when the keychain password is changed.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var passwordChangedEventMask: SecKeychainEventMask { get }
```

