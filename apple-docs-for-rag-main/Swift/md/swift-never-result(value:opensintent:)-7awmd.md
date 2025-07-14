

- Swift
- Never
-  result(value:opensIntent:) 

Type Method

# result(value:opensIntent:)

Indicates the `AppIntent` finished performing

SwiftAppIntentsiOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
static func result(
    value: Value,
    opensIntent: some AppIntent
) -> Self where Self == IntentResultContainer, Value : _IntentValue
```

## Parameters 

`value`  

The value produced by the `AppIntent`

`opensIntent`  

An `AppIntent` to shows the result of current intent

