

- App Intents
- IntentResultContainer
-  result(value:opensIntent:dialog:) 

Type Method

# result(value:opensIntent:dialog:)

Indicates the `AppIntent` finished performing

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func result(
    value: Value,
    opensIntent: OpensAppIntent,
    dialog: IntentDialog
) -> Self where Self == IntentResultContainer, Value : _IntentValue, OpensAppIntent : AppIntent
```

## Parameters 

`value`  

The value produced by the `AppIntent`

`opensIntent`  

An `AppIntent` to shows the result of current intent

`dialog`  

A custom success dialog

