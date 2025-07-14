

- SecureElementCredential
- CredentialSession
-  endWiredMode() 

Instance Method

# endWiredMode()

Ends wired mode and returns to management state.

iOS 18.1+iPadOS 18.1+

``` source
func endWiredMode() async throws
```

## Mentioned in 

Accessing and using secure element credentials

## Discussion

The credential session state must be CredentialSession.State.wired(credential:) prior to calling this method.

## See Also

### Performing wired mode actions

func performWiredTransaction(using: CredentialSession.Credential, over: UIScene, instanceAID: Data) async throws

Enters wired mode with user authentication.

func enterWiredMode(using: CredentialSession.Credential) async throws

Enters wired mode to perform maintenance operations with the given credential.

func transceive(Data) async throws -> Data

Send a wired command Application Protocol Data Unit (APDU) to the credential.

