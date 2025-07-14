

- ManagedAppDistribution
-  ManagedAppView 

Structure

# ManagedAppView

A view that displays a managed app.

ManagedAppDistributionSwiftUIiOS 17.2+iPadOS 17.2+

``` source
@MainActor @preconcurrency
struct ManagedAppView
```

## Topics

### Creating a view

init(app: ManagedApp)

Create a managed app view from a managed app.

### Getting the properties

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

struct ManagedContentView

struct ManagedContentOfferState

struct ManagedContentStyle

A type that applies a custom appearance to the managed content view.

