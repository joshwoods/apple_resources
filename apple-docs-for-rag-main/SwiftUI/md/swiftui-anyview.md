

- SwiftUI
-  AnyView 

Structure

# AnyView

A type-erased view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct AnyView
```

## Overview

An `AnyView` allows changing the type of view used in a given view hierarchy. Whenever the type of view used with an `AnyView` changes, the old hierarchy is destroyed and a new hierarchy is created for the new type.

## Topics

### Creating a view

init&lt;V>(V)

Create an instance that type-erases `view`.

init&lt;V>(erasing: V)

## Relationships

### Conforms To

- View

## See Also

### Supporting view types

struct EmptyView

A view that doesn’t contain any content.

struct EquatableView

A view type that compares itself against its previous value and prevents its child updating if its new value is the same as its old value.

struct SubscriptionView

A view that subscribes to a publisher with an action.

struct TupleView

A View created from a swift tuple of View values.

