

- Swift
- Never
-  result(value:opensIntent:dialog:) 

Type Method

# result(value:opensIntent:dialog:)

Indicates the `AppIntent` finished performing

SwiftAppIntentsiOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
static func result(
    value: Value,
    opensIntent: some AppIntent,
    dialog: IntentDialog
) -> Self where Self == IntentResultContainer, Value : _IntentValue
```

## Parameters 

`value`  

The value produced by the `AppIntent`

`opensIntent`  

An `AppIntent` to shows the result of current intent

`dialog`  

A custom success dialog

