

- Authentication Services
-  ASAuthorizationPublicKeyCredentialPRFAssertionOutput 

Structure

# ASAuthorizationPublicKeyCredentialPRFAssertionOutput

The outputs of the WebAuthentication PRF extension, when requested during an assertion. This object represents one or two SymmetricKeys which are available anywhere the passkey can be used. These are general purpose keys which can be used for application-specific needs, such as encryption of user data. These keys should not be stored or exported. They should only ever be derived as the result of an assertion operation, and then discarded when finished.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct ASAuthorizationPublicKeyCredentialPRFAssertionOutput
```

## Topics

### Initializers

init(first: SymmetricKey, second: SymmetricKey?)

### Instance Properties

let first: SymmetricKey

A SymmetricKey that is unique to this passkey and derived from `input1`.

let second: SymmetricKey?

A second SymmetricKey that is unique to this passkey, and derived from `input2` if it was specified. If `input2` was not specified, this will be nil.

