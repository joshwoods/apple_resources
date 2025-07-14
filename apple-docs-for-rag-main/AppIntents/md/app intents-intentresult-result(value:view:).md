

- App Intents
- IntentResult
-  result(value:view:) 

Type Method

# result(value:view:)

Indicates the `AppIntent` finished performing

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func result(
    value: Value,
    view: Content = EmptyView()
) -> Self where Self == IntentResultContainer, Value : _IntentValue, Content : View
```

## Parameters 

`value`  

The value produced by the `AppIntent`

`view`  

A custom View to display the result

