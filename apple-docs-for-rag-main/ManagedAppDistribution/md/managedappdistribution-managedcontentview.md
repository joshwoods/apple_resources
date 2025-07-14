

- ManagedAppDistribution
-  ManagedContentView 

Structure

# ManagedContentView

ManagedAppDistributionSwiftUIiOS 17.2+iPadOS 17.2+

``` source
@MainActor @preconcurrency
struct ManagedContentView where Icon : View
```

## Topics

### Creating views

init(primaryLabel: LocalizedStringKey, secondaryLabel: LocalizedStringKey, tertiaryLabel: LocalizedStringKey, quaternaryLabel: LocalizedStringKey, offerState: ManagedContentOfferState, offerAction: (ManagedContentOfferState) -> Void, icon: () -> Icon)

Create a view with the layout of a managed app view and customized labels using localized string keys.

init(primaryLabel: any StringProtocol, secondaryLabel: any StringProtocol, tertiaryLabel: any StringProtocol, quaternaryLabel: any StringProtocol, offerState: ManagedContentOfferState, offerAction: (ManagedContentOfferState) -> Void, icon: () -> Icon)

Create a content view with the layout of a managed app view and customized labels using strings.

### Inspecting the view

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

### View creation

struct ManagedAppView

A view that displays a managed app.

struct ManagedContentOfferState

struct ManagedContentStyle

A type that applies a custom appearance to the managed content view.

