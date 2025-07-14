

- Foundation
- URLCredential
- URLCredential.Persistence
-  URLCredential.Persistence.synchronizable 

Case

# URLCredential.Persistence.synchronizable

The credential should be stored permanently in the keychain, and in addition should be distributed to other devices based on the owning Apple ID.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case synchronizable
```

## See Also

### Persistence strategies

case none

The credential should not be stored.

case forSession

The credential should be stored only for this session.

case permanent

The credential should be stored in the keychain.

case none

The credential should not be stored.

case forSession

The credential should be stored only for this session.

case permanent

The credential should be stored in the keychain.

