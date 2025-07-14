

- App Intents
- SetFocusFilterIntent
-  suggestedFocusFilters(for:) 

Type Method

# suggestedFocusFilters(for:)

You can implement this method to return a list of suggested focus configurations. This is useful when the suggested focus configurations are different from the configuration when the focus is turned off.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func suggestedFocusFilters(for context: FocusFilterSuggestionContext) async -> [Self]
```

**Required** Default implementation provided.

## Parameters 

`context`  

The focus configuration context which the suggested configurations could be determined from.

## Return Value

A list of suggested focus configurations where the first one is the most suggested configuration. Returns an empty array if there is no suggested focus configurations. The system will use the default value per parameters in this case.

## Default Implementations

### SetFocusFilterIntent Implementations

static func suggestedFocusFilters(for: FocusFilterSuggestionContext) async -> [Self]

You can implement this method to return a list of suggested focus configurations. This is useful when the suggested focus configurations are different from the configuration when the focus is turned off.

## See Also

### Getting the current app configuration

static var current: Self

