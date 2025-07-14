

- Authentication Services
-  ASAuthorizationPublicKeyCredentialPRFRegistrationInput 

Structure

# ASAuthorizationPublicKeyCredentialPRFRegistrationInput

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ASAuthorizationPublicKeyCredentialPRFRegistrationInput
```

## Topics

### Instance Properties

let inputValues: ASAuthorizationPublicKeyCredentialPRFRegistrationInput.InputValues?

If specified, the input values to use when generating the PRF extension. If not specified, the output will only indicate whether the extension is supported.

let shouldCheckForSupport: Bool

### Type Aliases

typealias InputValues

### Type Properties

static var checkForSupport: ASAuthorizationPublicKeyCredentialPRFRegistrationInput

Check for whether the extension is supported for the newly created passkey.

### Type Methods

static func inputValues(ASAuthorizationPublicKeyCredentialPRFRegistrationInput.InputValues) -> ASAuthorizationPublicKeyCredentialPRFRegistrationInput

The inputs for the PRF extension, to evaluate if the new passkey supports this extension.

