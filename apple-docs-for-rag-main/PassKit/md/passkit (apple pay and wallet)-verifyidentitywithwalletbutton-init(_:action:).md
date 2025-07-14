

- PassKit (Apple Pay and Wallet)
- VerifyIdentityWithWalletButton
-  init(\_:action:) 

Initializer

# init(\_:action:)

Creates a verify identity button that starts the identity authorization flow.

PassKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
nonisolated
init(
    _ label: VerifyIdentityWithWalletButtonLabel = .verifyIdentity,
    action: @escaping () -> Void
)
```

Available when `Fallback` is `EmptyView`.

## Parameters 

`label`  

The button’s label.

`action`  

The action to perform when a person taps the button.

## See Also

### Creating the button

init(VerifyIdentityWithWalletButtonLabel, request: PKIdentityRequest, onCompletion: (Result&lt;PKIdentityDocument, any Error>) -> Void)

Creates a verify identity button that starts the identity authorization flow, with a completion handler.

init(VerifyIdentityWithWalletButtonLabel, request: PKIdentityRequest, onCompletion: (Result&lt;PKIdentityDocument, any Error>) -> Void, fallback: () -> Fallback)

Creates a verify identity button that starts the identity authorization flow, with a fallback view to use if the app can’t start the flow.

