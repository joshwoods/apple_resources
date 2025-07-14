

- Authentication Services
- ASCredentialProviderExtensionContext
-  completeRegistrationRequest(using:completionHandler:) 

Instance Method

# completeRegistrationRequest(using:completionHandler:)

Complete the registration request by providing the newly-created passkey credential.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
func completeRegistrationRequest(
    using credential: ASPasskeyRegistrationCredential,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
func completeRegistrationRequest(using credential: ASPasskeyRegistrationCredential) async -> Bool
```

## Parameters 

`credential`  

The credential your extension created in response to the registration request.

`completionHandler`  

An optional block your extension can provide to perform any cleanup work after the system has used the credential. The expired parameter is true if the system decides to prematurely end a previous non-expiration invocation of the completion handler.

## Discussion

The synchronous version of this method calls its completion handler with background priority.

## See Also

### Providing credentials

func completeRequest(withSelectedCredential: ASPasswordCredential, completionHandler: ((Bool) -> Void)?)

Provides the user-selected credential.

func completeAssertionRequest(using: ASPasskeyAssertionCredential, completionHandler: ((Bool) -> Void)?)

Complete the passkey assertion request by providing the user-selected passkey credential.

func completeOneTimeCodeRequest(using: ASOneTimeCodeCredential, completionHandler: ((Bool) -> Void)?)

Provides the user-selected one-time passcode (OTP).

class ASPasswordCredential

A password credential.

class ASPasskeyAssertionCredential

A passkey assertion credential.

class ASPasskeyRegistrationCredential

A passkey registration credential.

class ASOneTimeCodeCredential

A one-time passcode (OTP) credential.

