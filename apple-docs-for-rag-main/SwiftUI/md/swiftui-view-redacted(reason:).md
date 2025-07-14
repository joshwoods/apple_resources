

- SwiftUI
- View
-  redacted(reason:) 

Instance Method

# redacted(reason:)

Adds a reason to apply a redaction to this view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func redacted(reason: RedactionReasons) -> some View
```

## Discussion

Adding a redaction is an additive process: any redaction provided will be added to the reasons provided by the parent.

## See Also

### Redacting private content

Designing your app for the Always On state

Customize your watchOS app’s user interface for continuous display.

func privacySensitive(Bool) -> some View

Marks the view as containing sensitive, private user data.

func unredacted() -> some View

Removes any reason to apply a redaction to this view hierarchy.

var redactionReasons: RedactionReasons

The current redaction reasons applied to the view hierarchy.

var isSceneCaptured: Bool

The current capture state.

struct RedactionReasons

The reasons to apply a redaction to data displayed on screen.

