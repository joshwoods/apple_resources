

- SecureElementCredential
- CredentialSession
-  state 

Instance Property

# state

The current state of the session.

iOS 18.1+iPadOS 18.1+

``` source
var state: CredentialSession.State { get async }
```

## Mentioned in 

Accessing and using secure element credentials

## Discussion

Sessions start in the CredentialSession.State.management state. Calls to the wired or card emulation APIs change the state to CredentialSession.State.wired(credential:) or CredentialSession.State.cardEmulation(credential:). Leaving wired or card emulation mode returns the state to CredentialSession.State.management.

Explicitly invalidating the session, encountering an error, or the app entering the background changes the state to CredentialSession.State.invalid. An invalid session can’t return to one of the other states.

## See Also

### Accessing the session state

enum State

An enumeration of the possible states of a card session.

