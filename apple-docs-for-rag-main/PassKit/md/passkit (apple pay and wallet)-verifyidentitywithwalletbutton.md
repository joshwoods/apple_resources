

- PassKit (Apple Pay and Wallet)
-  VerifyIdentityWithWalletButton 

Structure

# VerifyIdentityWithWalletButton

A view that displays a button for identity verification.

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
struct VerifyIdentityWithWalletButton where Fallback : View
```

## Topics

### Creating the button

init(VerifyIdentityWithWalletButtonLabel, action: () -> Void)

Creates a verify identity button that starts the identity authorization flow.

init(VerifyIdentityWithWalletButtonLabel, request: PKIdentityRequest, onCompletion: (Result&lt;PKIdentityDocument, any Error>) -> Void)

Creates a verify identity button that starts the identity authorization flow, with a completion handler.

init(VerifyIdentityWithWalletButtonLabel, request: PKIdentityRequest, onCompletion: (Result&lt;PKIdentityDocument, any Error>) -> Void, fallback: () -> Fallback)

Creates a verify identity button that starts the identity authorization flow, with a fallback view to use if the app can’t start the flow.

## Relationships

### Conforms To

- Sendable
- View

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

struct VerifyIdentityWithWalletButtonLabel

A type that represents the label you use with a verify identity button.

struct VerifyIdentityWithWalletButtonStyle

A type that represents the style you use with a verify identity button.

