

- Authentication Services
-  ASAuthorizationPublicKeyCredentialPRFAssertionInput 

Structure

# ASAuthorizationPublicKeyCredentialPRFAssertionInput

This type represents the inputs for the WebAuthentication PRF extension, when used during assertion requests. The PRF extension lets you create general purpose SymmetricKeys from passkeys, which could useful for tasks such as encryption of user data. The same input values used with the same passkey will always produce the same SymmetricKey.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ASAuthorizationPublicKeyCredentialPRFAssertionInput
```

## Topics

### Structures

struct InputValues

These are the values which will be used as inputs to the salts for deriving the SymmetricKey. This type is analogous to AuthenticationExtensionsPRFValues in the WebAuthn spec.

### Instance Properties

let inputValues: ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues?

If specified, the input values to use when generating the PRF extension output. When also using `perCredentialInputValues`, the corresponding value from that dictionary may be used instead.

let perCredentialInputValues: [Data : ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues]?

A map of `credentialID`s to input values for the PRF extension. If the user selects a passkey which matches a `credentialID` in this dictionary, the corresponding input values will be used. If the selected passkey does not match and `inputValues` is non-nil, that will be used instead. Otherwise, no PRF output will be returned. When this value is non-empty, the request must specify `allowedCredentials`.

### Type Methods

static func inputValues(ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues, perCredentialInputValues: [Data : ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues]?) -> ASAuthorizationPublicKeyCredentialPRFAssertionInput

The inputs for the PRF extension.

static func perCredentialInputValues([Data : ASAuthorizationPublicKeyCredentialPRFAssertionInput.InputValues]) -> ASAuthorizationPublicKeyCredentialPRFAssertionInput

The inputs for the PRF extension, when not specifying general input values.

