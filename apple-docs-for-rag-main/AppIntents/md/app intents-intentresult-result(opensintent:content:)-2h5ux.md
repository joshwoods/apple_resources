

- App Intents
- IntentResult
-  result(opensIntent:content:) 

Type Method

# result(opensIntent:content:)

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func result(
    opensIntent: OpensAppIntent,
    @ViewBuilder content: () -> Content
) -> Self where Self == IntentResultContainer, OpensAppIntent : AppIntent, Content : View
```

