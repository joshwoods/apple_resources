

- App Intents
- IntentResult
-  result(opensIntent:dialog:view:) 

Type Method

# result(opensIntent:dialog:view:)

Indicates the `AppIntent` finished performing

AppIntentsSwiftUIiOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+tvOS 18.2+visionOS 2.2+watchOS 11.2+

``` source
static func result(
    opensIntent: some AppIntent,
    dialog: IntentDialog,
    view: Content = EmptyView()
) -> Self where Self == IntentResultContainer, Content : View
```

## Parameters 

`opensIntent`  

An `AppIntent` to shows the result of current intent

`dialog`  

A custom success dialog

`view`  

A custom View to display the result

