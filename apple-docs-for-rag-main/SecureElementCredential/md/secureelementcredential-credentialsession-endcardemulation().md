

- SecureElementCredential
- CredentialSession
-  endCardEmulation() 

Instance Method

# endCardEmulation()

Ends card emulation and transitions the session to management state.

SecureElementCredentialUIKitiOS 18.1+iPadOS 18.1+

``` source
func endCardEmulation() async throws
```

## Mentioned in 

Accessing and using secure element credentials

## See Also

### Performing card emulation

func performCardEmulationTransactionWithCurrentCredential(over: UIScene, options: CredentialSession.CardEmulationOptions) async throws

Activate the current credential in Wired mode to enter Card Emulation mode.

func performTransaction(using: CredentialSession.Credential, over: UIScene, options: CredentialSession.CardEmulationOptions) async throws

Prompts the user for authorization and then activate a credential for card emulation.

struct CardEmulationOptions

Options for customizing card emulation behavior.

