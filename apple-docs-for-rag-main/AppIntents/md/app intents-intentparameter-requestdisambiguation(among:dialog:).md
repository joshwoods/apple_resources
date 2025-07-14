

- App Intents
- IntentParameter
-  requestDisambiguation(among:dialog:) 

Instance Method

# requestDisambiguation(among:dialog:)

Request that the user disambiguate amongst an array of values for this parameter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final func requestDisambiguation(
    among itemsToDisambiguate: [Value.ValueType],
    dialog: IntentDialog? = nil
) async throws -> Value.ValueType
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Parameters 

`itemsToDisambiguate`  

The list of items to be presented to the user for disambiguation

`dialog`  

A custom dialog that may be used when prompting the user for the value

## Return Value

The value supplied by the user

## See Also

### Requesting disambiguation

func needsDisambiguationError(among: [Value.ValueType], dialog: IntentDialog?) -> AppIntentError

Returns a `restartPerform` error with context for the user to disambiguate amongst an array of values from for this parameter and re-perform the intent with the new value.

