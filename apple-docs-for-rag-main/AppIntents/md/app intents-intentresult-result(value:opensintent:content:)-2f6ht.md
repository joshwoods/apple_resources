

- App Intents
- IntentResult
-  result(value:opensIntent:content:) 

Type Method

# result(value:opensIntent:content:)

Indicates the `AppIntent` finished performing

AppIntentsSwiftUIiOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
static func result(
    value: Value,
    opensIntent: some AppIntent,
    @ViewBuilder content: () -> Content
) -> Self where Self == IntentResultContainer, Value : _IntentValue, Content : View
```

## Parameters 

`value`  

The value produced by the `AppIntent`

`opensIntent`  

An `AppIntent` to shows the result of current intent

`content`  

A custom View to display the result

