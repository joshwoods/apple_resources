

- FinanceKitUI
-  TransactionPicker 

Structure

# TransactionPicker

A view that displays a transaction picker for choosing transactions from FinanceKit.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
@MainActor @preconcurrency
struct TransactionPicker where Label : View
```

## Topics

### Initializers

init(selection: Binding&lt;[Transaction]>, label: () -> Label)

Creates a picker that selects a collection of transactions.

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

