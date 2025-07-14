

- SecureElementCredential
- CredentialSession
-  enterWiredMode(using:) 

Instance Method

# enterWiredMode(using:)

Enters wired mode to perform maintenance operations with the given credential.

iOS 18.1+iPadOS 18.1+

``` source
func enterWiredMode(using credential: CredentialSession.Credential) async throws
```

## Parameters 

`credential`  

The installed credential with which to enter wired mode.

## Discussion

You can call this method in any session state. If successful, the state transitions to CredentialSession.State.wired(credential:). The state transitions to CredentialSession.State.management if the call encounters a CredentialSession.ErrorCode.resourceUnavailable error; otherwise the state remains unchanged.

## See Also

### Performing wired mode actions

func performWiredTransaction(using: CredentialSession.Credential, over: UIScene, instanceAID: Data) async throws

Enters wired mode with user authentication.

func transceive(Data) async throws -> Data

Send a wired command Application Protocol Data Unit (APDU) to the credential.

func endWiredMode() async throws

Ends wired mode and returns to management state.

