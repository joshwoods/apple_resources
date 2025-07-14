

- Swift
- Never
-  result(value:opensIntent:) 

Type Method

# result(value:opensIntent:)

Indicates the `AppIntent` finished performing

SwiftAppIntentsiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func result(
    value: Value,
    opensIntent: OpensAppIntent
) -> Self where Self == IntentResultContainer, Value : _IntentValue, OpensAppIntent : AppIntent
```

## Parameters 

`value`  

The value produced by the `AppIntent`

`opensIntent`  

An `AppIntent` to shows the result of current intent

