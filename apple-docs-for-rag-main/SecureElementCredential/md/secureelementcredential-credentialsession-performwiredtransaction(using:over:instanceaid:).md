

- SecureElementCredential
- CredentialSession
-  performWiredTransaction(using:over:instanceAID:) 

Instance Method

# performWiredTransaction(using:over:instanceAID:)

Enters wired mode with user authentication.

SecureElementCredentialUIKitiOS 18.1+iPadOS 18.1+

``` source
func performWiredTransaction(
    using credential: CredentialSession.Credential,
    over scene: UIScene,
    instanceAID: Data
) async throws
```

## Parameters 

`credential`  

The credential to activate and transition into card emulation state with.

`scene`  

The UIScene the authentication sheet appears over.

`instanceAID`  

The applet instance identifier of the installed credential to authorize.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

If the user chooses to authorize, the specified instance will first have an auth token delivered by the broker interface on the Secure Element as described in the Apple Business Register Secure Element documents. Otherwise the session throws `userDeclined`.

Use the following flow to call this method:

1.  Call acquirePresentmentAssertion() before calling this function to ensure that UI from other applications’ payment tasks don’t interfere with this transaction.

2.  Relinquish the asssertion with relinquish() immediately prior to calling `performWiredTransaction(using:over:instanceAID:)`.

3.  After presenting the credential, call endWiredMode() to return to management mode.

4.  If you have further proprietary payment UI to perform, use acquirePresentmentAssertion() to re-acquire the assertion. Perform your tasks, then call relinquish() again. Re-acquiring the assertion is subject to the limit of two assertions in an 80-second span.

The credential session can be in any state when calling this method. If the call succeeds, the state transitions to CredentialSession.State.wired(credential:). The state transitions to CredentialSession.State.management if the call encounters a CredentialSession.ErrorCode.resourceUnavailable error; otherwise the state remains unchanged.

Important

Calling this method may generate a billable event to the credential provider.

## See Also

### Performing wired mode actions

func enterWiredMode(using: CredentialSession.Credential) async throws

Enters wired mode to perform maintenance operations with the given credential.

func transceive(Data) async throws -> Data

Send a wired command Application Protocol Data Unit (APDU) to the credential.

func endWiredMode() async throws

Ends wired mode and returns to management state.

