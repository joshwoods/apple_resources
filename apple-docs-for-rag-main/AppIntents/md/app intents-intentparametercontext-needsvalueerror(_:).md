

- App Intents
- IntentParameterContext
-  needsValueError(\_:) 

Instance Method

# needsValueError(\_:)

Returns a `restartPerform` error with context to request a value from the user for this parameter and re-perform the intent with the new value.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func needsValueError(_ dialog: IntentDialog? = nil) -> AppIntentError
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Parameters 

`dialog`  

A custom dialog that may be used when prompting the user for the value

## Return Value

An error that should be thrown within the intent `perform()` method.

