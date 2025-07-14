

- SecureElementCredential
- CredentialSession
- CredentialSession.Event
-  CredentialSession.Event.sessionInvalidated(reason:) 

Case

# CredentialSession.Event.sessionInvalidated(reason:)

The session became invalidated.

iOS 18.1+iPadOS 18.1+

``` source
case sessionInvalidated(reason: CredentialSession.ErrorCode)
```

## Discussion

The associated value `reason` provides a reason for the invalidation.

## See Also

### Invalidation events

enum ErrorCode

An error encountered by a credential session.

