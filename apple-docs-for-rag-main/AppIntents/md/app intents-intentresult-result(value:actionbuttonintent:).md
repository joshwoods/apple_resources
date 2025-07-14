

- App Intents
- IntentResult
-  result(value:actionButtonIntent:) 

Type Method

# result(value:actionButtonIntent:)

Indicates the Intent finished performing with an `AppIntent` to continue with

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func result(
    value: Value,
    actionButtonIntent: Intent
) -> Self where Self == IntentResultContainer, Value : _IntentValue, Intent : AppIntent
```

## Parameters 

`value`  

The value produced by the `AppIntent`

