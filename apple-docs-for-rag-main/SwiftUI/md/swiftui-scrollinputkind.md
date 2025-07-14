

- SwiftUI
-  ScrollInputKind 

Structure

# ScrollInputKind

Inputs used to scroll views.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct ScrollInputKind
```

## Topics

### Type Properties

static let handGestureShortcut: ScrollInputKind

A finger or wrist movement that the user can perform in order to scroll a view.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Managing scrolling for different inputs

func scrollInputBehavior(ScrollInputBehavior, for: ScrollInputKind) -> some View

Enables or disables scrolling in scrollable views when using particular inputs.

struct ScrollInputBehavior

A type that defines whether input should scroll a view.

