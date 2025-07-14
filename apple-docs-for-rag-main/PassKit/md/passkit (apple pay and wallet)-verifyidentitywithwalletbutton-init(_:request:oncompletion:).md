

- PassKit (Apple Pay and Wallet)
- VerifyIdentityWithWalletButton
-  init(\_:request:onCompletion:) 

Initializer

# init(\_:request:onCompletion:)

Creates a verify identity button that starts the identity authorization flow, with a completion handler.

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
nonisolated
init(
    _ label: VerifyIdentityWithWalletButtonLabel = .verifyIdentity,
    request: PKIdentityRequest,
    onCompletion: @escaping (Result) -> Void
)
```

Available when `Fallback` is `EmptyView`.

## Parameters 

`label`  

The button’s label.

`request`  

The identity request to make when a person taps the button.

`onCompletion`  

The completion handler the framework calls when finishing the authorization flow.

`result`  
A result that contains an identity document, if successful; otherwise, an error.

## See Also

### Creating the button

init(VerifyIdentityWithWalletButtonLabel, action: () -> Void)

Creates a verify identity button that starts the identity authorization flow.

init(VerifyIdentityWithWalletButtonLabel, request: PKIdentityRequest, onCompletion: (Result&lt;PKIdentityDocument, any Error>) -> Void, fallback: () -> Fallback)

Creates a verify identity button that starts the identity authorization flow, with a fallback view to use if the app can’t start the flow.

