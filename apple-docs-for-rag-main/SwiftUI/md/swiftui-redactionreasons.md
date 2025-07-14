

- SwiftUI
-  RedactionReasons 

Structure

# RedactionReasons

The reasons to apply a redaction to data displayed on screen.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct RedactionReasons
```

## Topics

### Getting redaction reasons

static let invalidated: RedactionReasons

Displayed data should appear as invalidated and pending a new update.

static let placeholder: RedactionReasons

Displayed data should appear as generic placeholders.

static let privacy: RedactionReasons

Displayed data should be obscured to protect private information.

### Creating redaction reasons

init(rawValue: Int)

Creates a new set from a raw value.

let rawValue: Int

The raw value.

## Relationships

### Conforms To

- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Redacting private content

Designing your app for the Always On state

Customize your watchOS app’s user interface for continuous display.

func privacySensitive(Bool) -> some View

Marks the view as containing sensitive, private user data.

func redacted(reason: RedactionReasons) -> some View

Adds a reason to apply a redaction to this view hierarchy.

func unredacted() -> some View

Removes any reason to apply a redaction to this view hierarchy.

var redactionReasons: RedactionReasons

The current redaction reasons applied to the view hierarchy.

var isSceneCaptured: Bool

The current capture state.

