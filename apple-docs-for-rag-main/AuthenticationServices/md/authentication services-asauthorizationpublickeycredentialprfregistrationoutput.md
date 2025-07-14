

- Authentication Services
-  ASAuthorizationPublicKeyCredentialPRFRegistrationOutput 

Structure

# ASAuthorizationPublicKeyCredentialPRFRegistrationOutput

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ASAuthorizationPublicKeyCredentialPRFRegistrationOutput
```

## Topics

### Initializers

init(first: SymmetricKey, second: SymmetricKey?)

This method should only be called if input values were provided with the registration request. Otherwise, use `.supported` or `.unsupported`.

### Instance Properties

let first: SymmetricKey?

A SymmetricKey that is unique to this passkey and derived from `input1`, if it was specified.

let isSupported: Bool

let second: SymmetricKey?

A second SymmetricKey that is unique to this passkey, and derived from `input2` if it was specified.

### Type Properties

static var supported: ASAuthorizationPublicKeyCredentialPRFRegistrationOutput

static var unsupported: ASAuthorizationPublicKeyCredentialPRFRegistrationOutput

