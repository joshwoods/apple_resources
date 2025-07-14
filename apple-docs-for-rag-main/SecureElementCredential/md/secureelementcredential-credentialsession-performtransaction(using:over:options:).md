

- SecureElementCredential
- CredentialSession
-  performTransaction(using:over:options:) 

Instance Method

# performTransaction(using:over:options:)

Prompts the user for authorization and then activate a credential for card emulation.

SecureElementCredentialUIKitiOS 18.1+iPadOS 18.1+

``` source
func performTransaction(
    using credential: CredentialSession.Credential,
    over scene: UIScene,
    options: CredentialSession.CardEmulationOptions = .init()
) async throws
```

## Parameters 

`credential`  

The credential to activate and transition into card emulation state with.

`scene`  

The UIScene the authentication sheet appears over.

`options`  

Options with which to transition the credential to card emulation mode.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

1.  Call acquirePresentmentAssertion() before calling this function to ensure that UI from other applications’ payment tasks don’t interfere with this transaction.

2.  Relinquish the asssertion with relinquish() immediately prior to calling `performTransaction(using:over:options:)`.

3.  After presenting the credential, call endCardEmulation() to return to management mode.

4.  If you have further proprietary payment UI to perform, use acquirePresentmentAssertion() to re-acquire the assertion. Perform your tasks, then call relinquish() again. Re-acquiring the assertion is subject to the limit of two assertions in an 80-second span.

The credential session state must be CredentialSession.State.wired(credential:) prior to calling this method. The state transitions to CredentialSession.State.management if the call encounters a CredentialSession.ErrorCode.resourceUnavailable error; otherwise the state remains unchanged.

If this call succeeds the credential session state transitions to the CredentialSession.State.cardEmulation(credential:) state. The session also publishes a CredentialSession.Event.fieldStateChanged(info:) event.

If not ended sooner, card emulation expires after 60 seconds and the credential session publishes a CredentialSession.Event.cardEmulationTimeout event.

Important

Calling this method may generate a billable event to the credential provider.

## See Also

### Performing card emulation

func performCardEmulationTransactionWithCurrentCredential(over: UIScene, options: CredentialSession.CardEmulationOptions) async throws

Activate the current credential in Wired mode to enter Card Emulation mode.

struct CardEmulationOptions

Options for customizing card emulation behavior.

func endCardEmulation() async throws

Ends card emulation and transitions the session to management state.

