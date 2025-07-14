

- SecureElementCredential
- CredentialSession
- CredentialSession.Event
-  CredentialSession.Event.cardEmulationTimeout 

Case

# CredentialSession.Event.cardEmulationTimeout

The session’s card emulation timer expired.

iOS 18.1+iPadOS 18.1+

``` source
case cardEmulationTimeout
```

## Discussion

This event the session’s state back to CredentialSession.State.management.

When handling this event, SwiftUI applications must invalidate the CredentialTransaction.Configuration requested for this transaction.

## See Also

### Timeout events

case presentmentIntentAssertionTimeout

The session’s presentment intent assertion timed out.

