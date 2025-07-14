

- Security
- SecKeychainEvent
-  SecKeychainEvent.unlockEvent 

Case

# SecKeychainEvent.unlockEvent

Indicates a keychain was successfully unlocked.

Mac Catalyst 13.0+macOS 10.0+

``` source
case unlockEvent
```

## Discussion

It is impossible to distinguish between an unlock event caused by an explicit request and one that occurred automatically because the keychain was needed to perform an operation. In either case, however, the `pid` parameter in the `SecKeychainCallbackInfo` structure does return the ID of the process whose actions caused the unlock event.

