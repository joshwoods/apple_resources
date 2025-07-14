

- App Intents
- IntentResult
-  result(opensIntent:content:) 

Type Method

# result(opensIntent:content:)

Indicates the `AppIntent` finished performing

AppIntentsSwiftUIiOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
static func result(
    opensIntent: some AppIntent,
    @ViewBuilder content: () -> Content
) -> Self where Self == IntentResultContainer, Content : View
```

## Parameters 

`opensIntent`  

An `AppIntent` to shows the result of current intent

`content`  

A custom View to display the result

