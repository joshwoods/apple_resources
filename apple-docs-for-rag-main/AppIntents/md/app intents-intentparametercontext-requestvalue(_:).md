

- App Intents
- IntentParameterContext
-  requestValue(\_:) 

Instance Method

# requestValue(\_:)

Request a value from the user for this parameter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func requestValue(_ dialog: IntentDialog? = nil) async throws -> Value.ValueType
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

## Parameters 

`dialog`  

A custom dialog that may be used when prompting the user for the value

## Return Value

The value supplied by the user

