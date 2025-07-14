

- SecureElementCredential
- CredentialSession
-  CredentialSession.CardEmulationOptions 

Structure

# CredentialSession.CardEmulationOptions

Options for customizing card emulation behavior.

iOS 18.1+iPadOS 18.1+

``` source
struct CardEmulationOptions
```

## Topics

### Creating an options instance

init()

## Relationships

### Conforms To

- Sendable

## See Also

### Performing card emulation

func performCardEmulationTransactionWithCurrentCredential(over: UIScene, options: CredentialSession.CardEmulationOptions) async throws

Activate the current credential in Wired mode to enter Card Emulation mode.

func performTransaction(using: CredentialSession.Credential, over: UIScene, options: CredentialSession.CardEmulationOptions) async throws

Prompts the user for authorization and then activate a credential for card emulation.

func endCardEmulation() async throws

Ends card emulation and transitions the session to management state.

