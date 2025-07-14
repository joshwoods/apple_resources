

- App Intents
- IntentParameter
-  needsDisambiguationError(among:dialog:) 

Instance Method

# needsDisambiguationError(among:dialog:)

Returns a `restartPerform` error with context for the user to disambiguate amongst an array of values from for this parameter and re-perform the intent with the new value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final func needsDisambiguationError(
    among itemsToDisambiguate: [Value.ValueType],
    dialog: IntentDialog? = nil
) -> AppIntentError
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Parameters 

`itemsToDisambiguate`  

The list of items to be presented to the user for disambiguation

`dialog`  

A custom dialog that may be used when prompting the user for the value

## Return Value

An error that should be thrown within the intent `perform()` method.

## See Also

### Requesting disambiguation

func requestDisambiguation(among: [Value.ValueType], dialog: IntentDialog?) async throws -> Value.ValueType

Request that the user disambiguate amongst an array of values for this parameter.

