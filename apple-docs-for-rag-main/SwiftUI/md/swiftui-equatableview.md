

- SwiftUI
-  EquatableView 

Structure

# EquatableView

A view type that compares itself against its previous value and prevents its child updating if its new value is the same as its old value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct EquatableView where Content : Equatable, Content : View
```

## Topics

### Creating an equatable view

init(content: Content)

var content: Content

## Relationships

### Conforms To

- View

## See Also

### Supporting view types

struct AnyView

A type-erased view.

struct EmptyView

A view that doesn’t contain any content.

struct SubscriptionView

A view that subscribes to a publisher with an action.

struct TupleView

A View created from a swift tuple of View values.

