

- App Intents
- IntentResult
-  result(dialog:content:) 

Type Method

# result(dialog:content:)

Indicates the `AppIntent` finished performing

AppIntentsSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func result(
    dialog: IntentDialog,
    @ViewBuilder content: () -> Content
) -> Self where Self == IntentResultContainer, Content : View
```

## Parameters 

`dialog`  

A custom success dialog

`content`  

A custom View to display the result

