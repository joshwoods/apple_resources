

- Authentication Services
- ASAuthorizationPublicKeyCredentialPRFAssertionInput
-  ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues 

Structure

# ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues

These are the values which will be used as inputs to the salts for deriving the SymmetricKey. This type is analogous to AuthenticationExtensionsPRFValues in the WebAuthn spec.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct InputValues
```

## Topics

### Initializers

init(saltInput1: Data, saltInput2: Data?)

### Instance Properties

var saltInput1: Data

var saltInput2: Data?

### Type Methods

static func saltInput1(Data, saltInput2: Data?) -> ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues

The inputs for generating the PRF output secrets.

