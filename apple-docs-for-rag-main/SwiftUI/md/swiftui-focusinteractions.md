

- SwiftUI
-  FocusInteractions 

Structure

# FocusInteractions

Values describe different focus interactions that a view can support.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct FocusInteractions
```

## Topics

### Creating the interaction types

static var automatic: FocusInteractions

The view supports whatever focus-driven interactions are commonly expected for interactive content on the current platform.

static let activate: FocusInteractions

The view has a primary action that can be activated via focus gestures.

static let edit: FocusInteractions

The view captures input from non-spatial sources like a keyboard or Digital Crown.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Indicating that a view can receive focus

func focusable(Bool) -> some View

Specifies if the view is focusable.

func focusable(Bool, interactions: FocusInteractions) -> some View

Specifies if the view is focusable, and if so, what focus-driven interactions it supports.

