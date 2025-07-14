

- SwiftUI
-  DefaultFocusEvaluationPriority 

Structure

# DefaultFocusEvaluationPriority

Prioritizations for default focus preferences when evaluating where to move focus in different circumstances.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct DefaultFocusEvaluationPriority
```

## Topics

### Getting the priorities

static let automatic: DefaultFocusEvaluationPriority

Use the default focus preference when focus moves into the affected branch automatically, but ignore it when the movement is driven by a user-initiated navigation command.

static let userInitiated: DefaultFocusEvaluationPriority

Always use the default focus preference when focus moves into the affected branch.

## Relationships

### Conforms To

- Sendable

## See Also

### Controlling default focus

func prefersDefaultFocus(Bool, in: Namespace.ID) -> some View

Indicates that the view should receive focus by default for a given namespace.

func defaultFocus&lt;V>(FocusState&lt;V>.Binding, V, priority: DefaultFocusEvaluationPriority) -> some View

Defines a region of the window in which default focus is evaluated by assigning a value to a given focus state binding.

