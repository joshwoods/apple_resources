

- SecureElementCredential
- CredentialSession
-  transceive(\_:) 

Instance Method

# transceive(\_:)

Send a wired command Application Protocol Data Unit (APDU) to the credential.

iOS 18.1+iPadOS 18.1+

``` source
func transceive(_ data: Data) async throws -> Data
```

## Parameters 

`data`  

The APDU as a Data instance.

## Return Value

A response APDU.

## Mentioned in 

Accessing and using secure element credentials

## Discussion

Before calling this method, make sure the credential session state is CredentialSession.State.wired(credential:). The state transitions to CredentialSession.State.management if the call encounters a CredentialSession.ErrorCode.resourceUnavailable error; otherwise the state remains unchanged.

Note

When performing a transceive(_:) call, the system grants your app a 15-second grace period from invalidating the session, in the event your app goes into the background.

## See Also

### Performing wired mode actions

func performWiredTransaction(using: CredentialSession.Credential, over: UIScene, instanceAID: Data) async throws

Enters wired mode with user authentication.

func enterWiredMode(using: CredentialSession.Credential) async throws

Enters wired mode to perform maintenance operations with the given credential.

func endWiredMode() async throws

Ends wired mode and returns to management state.

