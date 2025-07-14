

- SecureElementCredential
- CredentialTransaction
-  performCardEmulationTransactionWithCurrentCredential(options:) 

Instance Method

# performCardEmulationTransactionWithCurrentCredential(options:)

Activate the current credential to perform a transaction in card emulation mode.

SecureElementCredentialSwiftUIiOS 18.1+iPadOS 18.1+

``` source
func performCardEmulationTransactionWithCurrentCredential(options: CardEmulationOptions = .init()) async throws
```

## Parameters 

`options`  

The options to transition the credential to card emulation mode.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

Calling this method requires that the credential’s state is `wired`. If successful, the state transitions to CredentialSession.State.cardEmulation(credential:). If an error occurs, the state is unchanged, unless the error is CredentialSession.ErrorCode.resourceUnavailable, which transitions the state back to CredentialSession.State.management.

When you call this method, the following sequence of events takes place:

1.  The system prompts the user to authorize Card Emulation.

2.  The system deselects the instance on the wired interface.

3.  The system calls the broker interface with authorization information, if applicable. See the integration guide in the Apple Business Register.

4.  The system makes the instance available over the contactless interface and transitions the session to the card emulation state.

This process is guaranteed to preserve contents of the Clear On Reset buffer in the operating system running on the Secure Element. This allows you to create some context in wired mode that remains valid later in card emulation mode.

The caller needs to invoke invalidate() after completing each transaction.

Important

Calling this method may generate a billable event to the credential provider.

## See Also

### Performing transactions

func performTransaction(using: Credential, options: CardEmulationOptions) async throws

Prompts the user for authorization and then activates a credential for card emulation.

func performTransactionInWiredMode(using: Credential, instanceAID: Data) async throws

Enters wired mode to perform a transaction.

