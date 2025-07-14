

- SwiftUI
- EnvironmentValues
-  isSceneCaptured 

Instance Property

# isSceneCaptured

The current capture state.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+visionOS 1.0+

``` source
var isSceneCaptured: Bool { get set }
```

## Discussion

Use this value to determine whether the scene is actively being cloned to another destination (like during AirPlay) or is being mirrored or recorded.

Your app can respond to changes in this value to take appropriate action, like obscuring content.

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

struct RedactionReasons

The reasons to apply a redaction to data displayed on screen.

