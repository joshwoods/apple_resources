

- App Intents
- IntentResult
-  result(value:opensIntent:content:) 

Type Method

# result(value:opensIntent:content:)

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func result(
    value: Value,
    opensIntent: OpensAppIntent,
    @ViewBuilder content: () -> Content
) -> Self where Self == IntentResultContainer, Value : _IntentValue, OpensAppIntent : AppIntent, Content : View
```

