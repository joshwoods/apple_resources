

- App Intents
- IntentParameter
-  requestValue(\_:) 

Instance Method

# requestValue(\_:)

Request a value from the user for this parameter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final func requestValue(_ dialog: IntentDialog? = nil) async throws -> Value.ValueType
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Parameters 

`dialog`  

A custom dialog that may be used when prompting the user for the value

## Return Value

The value supplied by the user

## Mentioned in 

Adding parameters to an app intent

## See Also

### Requesting a value

func needsValueError(IntentDialog?) -> AppIntentError

Returns a `restartPerform` error with context to request a value from the user for this parameter and re-perform the intent with the new value.

