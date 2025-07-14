

- App Intents
- SetFocusFilterIntent
-  current 

Type Property

# current

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static var current: Self { get async throws }
```

## See Also

### Getting the current app configuration

static func suggestedFocusFilters(for: FocusFilterSuggestionContext) async -> [Self]

You can implement this method to return a list of suggested focus configurations. This is useful when the suggested focus configurations are different from the configuration when the focus is turned off.

**Required** Default implementation provided.

