

- SecureElementCredential
- CredentialTransaction
-  performTransactionInWiredMode(using:instanceAID:) 

Instance Method

# performTransactionInWiredMode(using:instanceAID:)

Enters wired mode to perform a transaction.

SecureElementCredentialSwiftUIiOS 18.1+iPadOS 18.1+

``` source
func performTransactionInWiredMode(
    using credential: Credential,
    instanceAID: Data
) async throws
```

## Parameters 

`credential`  

The installed credential to enter wired mode with.

`instanceAID`  

The instance applet instance identifier of the installed credential to authorize.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

After you call this method, the system shows an authorization screen to the person using the app. If they choose to authorize, the specified instance receives an authentication token. The instance receives this token through the broker interface on the Secure Element as described in the Apple Business Register Secure Element documents.

If the person using the app declines the authorization, the session throws CredentialSession.ErrorCode.accessDenied.

You can call this method in any session state. The state transitions to CredentialSession.State.wired(credential:) if successful. If an error occurs, the state is unchanged, unless the error is CredentialSession.ErrorCode.resourceUnavailable, which transitions the state back to CredentialSession.State.management.

The caller must invoke invalidate() after completing each transaction.

## See Also

### Performing transactions

func performTransaction(using: Credential, options: CardEmulationOptions) async throws

Prompts the user for authorization and then activates a credential for card emulation.

func performCardEmulationTransactionWithCurrentCredential(options: CardEmulationOptions) async throws

Activate the current credential to perform a transaction in card emulation mode.

