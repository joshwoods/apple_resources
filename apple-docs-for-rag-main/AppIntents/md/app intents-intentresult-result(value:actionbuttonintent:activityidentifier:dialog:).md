

- App Intents
- IntentResult
-  result(value:actionButtonIntent:activityIdentifier:dialog:) 

Type Method

# result(value:actionButtonIntent:activityIdentifier:dialog:)

Indicates the Intent finished performing with an `AppIntent` to continue with

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
static func result(
    value: Value,
    actionButtonIntent: Intent,
    activityIdentifier: String,
    dialog: IntentDialog
) -> Self where Self == IntentResultContainer, Value : _IntentValue, Intent : AppIntent
```

## Parameters 

`value`  

The value produced by the `AppIntent`

`dialog`  

A custom success dialog

