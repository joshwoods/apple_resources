

- App Intents
- IntentParameter
-  requestValue(\_:) Deprecated

Instance Method

# requestValue(\_:)

Request a value from the user for this parameter.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final func requestValue(_ dialog: IntentDialog? = nil) -> any Error
```

Available when `Value` conforms to `_IntentValue` and `Sendable`.

Deprecated

Use \`requestValue(\_:)\` or \`needsValueError(\_:)\` instead

