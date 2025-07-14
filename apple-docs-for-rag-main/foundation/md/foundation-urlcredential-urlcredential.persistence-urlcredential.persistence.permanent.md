

- Foundation
- URLCredential
- URLCredential.Persistence
-  URLCredential.Persistence.permanent 

Case

# URLCredential.Persistence.permanent

The credential should be stored in the keychain.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case permanent
```

## See Also

### Persistence strategies

case none

The credential should not be stored.

case forSession

The credential should be stored only for this session.

case synchronizable

The credential should be stored permanently in the keychain, and in addition should be distributed to other devices based on the owning Apple ID.

case none

The credential should not be stored.

case forSession

The credential should be stored only for this session.

case synchronizable

The credential should be stored permanently in the keychain, and in addition should be distributed to other devices based on the owning Apple ID.

