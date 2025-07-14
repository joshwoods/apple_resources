

- Security
- SecKeychainEventMask
-  trustSettingsChangedEventMask 

Type Property

# trustSettingsChangedEventMask

If the bit specified by this mask is set, your callback function is invoked when there is a change in certificate trust settings.

Mac Catalyst 13.0+macOS 10.0+

``` source
static var trustSettingsChangedEventMask: SecKeychainEventMask { get }
```

