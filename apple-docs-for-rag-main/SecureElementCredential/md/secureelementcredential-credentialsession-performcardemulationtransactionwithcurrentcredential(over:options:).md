

- SecureElementCredential
- CredentialSession
-  performCardEmulationTransactionWithCurrentCredential(over:options:) 

Instance Method

# performCardEmulationTransactionWithCurrentCredential(over:options:)

Activate the current credential in Wired mode to enter Card Emulation mode.

SecureElementCredentialUIKitiOS 18.1+iPadOS 18.1+

``` source
func performCardEmulationTransactionWithCurrentCredential(
    over scene: UIScene,
    options: CredentialSession.CardEmulationOptions = .init()
) async throws
```

## Parameters 

`scene`  

The UIScene the authentication sheet appears over.

`options`  

Options with which to transition the credential to card emulation mode.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

This call leads to the following sequence of events.

1.  Prompts the user to authorize Card Emulation.

2.  Deselects the instance on the wired interface.

3.  Calls the broker interface with authorization information (if applicable). See the integration guide in the Apple Business Register for more information about this interface.

4.  Makes the instance available over the contactless interface and transition the session to emulation state.

This process is guaranteed to preserve contents of the Clear On Reset buffer in the operating system running on the Secure Element. This allows you to create some context in wired mode that remains valid later in card emulation mode.

Use the following flow to call this method:

1.  Call acquirePresentmentAssertion() before calling this function to ensure that UI from other applications’ payment tasks don’t interfere with this transaction.

2.  Relinquish the asssertion with relinquish() immediately prior to calling `performCardEmulationTransactionWithCurrentCredential(over:options:)`.

3.  After presenting the credential, call endWiredMode() to return to management mode.

4.  If you have further proprietary payment UI to perform, use acquirePresentmentAssertion() to re-acquire the assertion. Perform your tasks, then call relinquish() again. Re-acquiring the assertion is subject to the limit of two assertions in an 80-second span.

The credential session state must be CredentialSession.State.wired(credential:) prior to calling this method. The state transitions to CredentialSession.State.management if the call encounters a CredentialSession.ErrorCode.resourceUnavailable error; otherwise the state remains unchanged.

Important

Calling this method may generate a billable event to the credential provider.

## See Also

### Performing card emulation

func performTransaction(using: CredentialSession.Credential, over: UIScene, options: CredentialSession.CardEmulationOptions) async throws

Prompts the user for authorization and then activate a credential for card emulation.

struct CardEmulationOptions

Options for customizing card emulation behavior.

func endCardEmulation() async throws

Ends card emulation and transitions the session to management state.

