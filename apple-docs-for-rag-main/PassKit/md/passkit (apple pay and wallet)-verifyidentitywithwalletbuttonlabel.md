

- PassKit (Apple Pay and Wallet)
-  VerifyIdentityWithWalletButtonLabel 

Structure

# VerifyIdentityWithWalletButtonLabel

A type that represents the label you use with a verify identity button.

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
struct VerifyIdentityWithWalletButtonLabel
```

## Topics

### Getting standard labels

static let `continue`: VerifyIdentityWithWalletButtonLabel

A button label that describes continuing with Apple Wallet.

static let verify: VerifyIdentityWithWalletButtonLabel

A button label that describes verifying with Apple Wallet.

static let verifyAge: VerifyIdentityWithWalletButtonLabel

A button label that describes verifying age with Apple Wallet.

static let verifyIdentity: VerifyIdentityWithWalletButtonLabel

A button label that describes verifying identity with Apple Wallet.

## See Also

### Identity sheet interactions and authorization

Requesting identity data from a Wallet pass

Initiate a request for identity information by prompting a user for permission and decrypting a response payload.

Verifying Wallet identity requests

Decrypt and verify an in-app presentment request on your server.

class PKIdentityAuthorizationController

An object that presents a sheet that prompts the user to allow a request for identity information.

class PKIdentityRequest

An object that represents a request for identity information from a Wallet pass.

class PKIdentityDocument

An object that represents the response to a request.

class PKIdentityElement

An object that represents the elements an app requests from identity documents.

class PKIdentityButton

An object that displays a button to trigger the identity verification flow.

struct VerifyIdentityWithWalletButton

A view that displays a button for identity verification.

struct VerifyIdentityWithWalletButtonStyle

A type that represents the style you use with a verify identity button.

