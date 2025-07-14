

- Swift
- Never
-  result(value:actionButtonIntent:activityIdentifier:) 

Type Method

# result(value:actionButtonIntent:activityIdentifier:)

Indicates the Intent finished performing with an `AppIntent` to continue with

SwiftAppIntentsiOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
static func result(
    value: Value,
    actionButtonIntent: Intent,
    activityIdentifier: String
) -> Self where Self == IntentResultContainer, Value : _IntentValue, Intent : AppIntent
```

## Parameters 

`value`  

The value produced by the `AppIntent`

