

- SecureElementCredential
- CredentialTransaction
-  performTransaction(using:options:) 

Instance Method

# performTransaction(using:options:)

Prompts the user for authorization and then activates a credential for card emulation.

SecureElementCredentialSwiftUIiOS 18.1+iPadOS 18.1+

``` source
func performTransaction(
    using credential: Credential,
    options: CardEmulationOptions = .init()
) async throws
```

## Parameters 

`credential`  

The credential to activate and transition into card emulation state.

`options`  

The options to activate the credential with, defaults to none.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

If this call succeeds, the session state trasitions to CredentialSession.State.cardEmulation(credential:), and the event stream publishes a CredentialSession.Event.fieldStateChanged(info:) event.

Card emulation ends after 60 seconds, at which point the the event stream publishes a CredentialSession.Event.cardEmulationTimeout event. If you complete your transaction before the timeout, call endCardEmulation() to exit card emulation mode.

The caller needs to invoke invalidate() after completing each transaction.

Important

Calling this method may generate a billable event to the credential provider.

## See Also

### Performing transactions

func performTransactionInWiredMode(using: Credential, instanceAID: Data) async throws

Enters wired mode to perform a transaction.

func performCardEmulationTransactionWithCurrentCredential(options: CardEmulationOptions) async throws

Activate the current credential to perform a transaction in card emulation mode.

