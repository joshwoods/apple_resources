

- Authentication Services
-  ASCredentialProviderExtensionContext 

Class

# ASCredentialProviderExtensionContext

A mechanism that credential provider extensions use to communicate with the system.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class ASCredentialProviderExtensionContext
```

## Topics

### Configuring the extension

func completeExtensionConfigurationRequest()

Completes the request to configure the extension.

### Providing credentials

func completeRequest(withSelectedCredential: ASPasswordCredential, completionHandler: ((Bool) -> Void)?)

Provides the user-selected credential.

func completeAssertionRequest(using: ASPasskeyAssertionCredential, completionHandler: ((Bool) -> Void)?)

Complete the passkey assertion request by providing the user-selected passkey credential.

func completeRegistrationRequest(using: ASPasskeyRegistrationCredential, completionHandler: ((Bool) -> Void)?)

Complete the registration request by providing the newly-created passkey credential.

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

### Providing text to AutoFill

func completeRequest(withTextToInsert: String, completionHandler: ((Bool) -> Void)?)

Provides the user-selected text.

### Canceling

func cancelRequest(withError: any Error)

Cancels the request.

## Relationships

### Inherits From

- NSExtensionContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Getting the extension context

var extensionContext: ASCredentialProviderExtensionContext

The context your credential provider extension uses to provide information to the system.

