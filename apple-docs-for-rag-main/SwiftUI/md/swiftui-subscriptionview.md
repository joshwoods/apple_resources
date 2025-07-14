

- SwiftUI
-  SubscriptionView 

Structure

# SubscriptionView

A view that subscribes to a publisher with an action.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct SubscriptionView where PublisherType : Publisher, Content : View, PublisherType.Failure == Never
```

## Topics

### Creating a subscription view

init(content: Content, publisher: PublisherType, action: (PublisherType.Output) -> Void)

### Managing the subscription

var publisher: PublisherType

The `Publisher` that is being subscribed.

var action: (PublisherType.Output) -> Void

The `Action` executed when `publisher` emits an event.

var content: Content

The content view.

## Relationships

### Conforms To

- View

## See Also

### Supporting view types

struct AnyView

A type-erased view.

struct EmptyView

A view that doesn’t contain any content.

struct EquatableView

A view type that compares itself against its previous value and prevents its child updating if its new value is the same as its old value.

struct TupleView

A View created from a swift tuple of View values.

