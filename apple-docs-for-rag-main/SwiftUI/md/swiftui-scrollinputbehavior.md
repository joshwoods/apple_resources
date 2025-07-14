

- SwiftUI
-  ScrollInputBehavior 

Structure

# ScrollInputBehavior

A type that defines whether input should scroll a view.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct ScrollInputBehavior
```

## Topics

### Type Properties

static let automatic: ScrollInputBehavior

Indicates that the system should determine whether the associated input scrolls a view.

static let disabled: ScrollInputBehavior

Indicates that the associated input should not scroll a view.

static let enabled: ScrollInputBehavior

Indicates that the associated input should scroll a view.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Managing scrolling for different inputs

func scrollInputBehavior(ScrollInputBehavior, for: ScrollInputKind) -> some View

Enables or disables scrolling in scrollable views when using particular inputs.

struct ScrollInputKind

Inputs used to scroll views.

