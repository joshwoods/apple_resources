

- FinanceKitUI
-  AddOrderToWalletButton 

Structure

# AddOrderToWalletButton

A button you use to add an order to a person’s Apple Wallet.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+

``` source
@MainActor @preconcurrency
struct AddOrderToWalletButton
```

## Topics

### Initializers

init(signedArchive: Data, onCompletion: (Result&lt;FinanceStore.SaveOrderResult, any Error>) -> Void)

Returns an initialized Add to Order Button.

### Instance Properties

var body: some View

The content and behavior of the view.

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Adding an order to Apple Wallet

struct AddOrderToWalletButtonStyle

Values that determine the style of an Add Order to Apple Wallet button.

