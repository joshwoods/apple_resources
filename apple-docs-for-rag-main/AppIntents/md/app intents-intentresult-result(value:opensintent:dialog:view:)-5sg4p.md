

- App Intents
- IntentResult
-  result(value:opensIntent:dialog:view:) 

Type Method

# result(value:opensIntent:dialog:view:)

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func result(
    value: Value,
    opensIntent: OpensAppIntent,
    dialog: IntentDialog,
    view: Content = EmptyView()
) -> Self where Self == IntentResultContainer, Value : _IntentValue, OpensAppIntent : AppIntent, Content : View
```

