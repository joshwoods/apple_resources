

- SwiftUI
- EnvironmentValues
-  redactionReasons 

Instance Property

# redactionReasons

The current redaction reasons applied to the view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var redactionReasons: RedactionReasons { get set }
```

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

var isSceneCaptured: Bool

The current capture state.

struct RedactionReasons

The reasons to apply a redaction to data displayed on screen.

