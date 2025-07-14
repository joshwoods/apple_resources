

- Swift
- Never
-  result(opensIntent:dialog:) 

Type Method

# result(opensIntent:dialog:)

Indicates the `AppIntent` finished performing

SwiftAppIntentsiOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
static func result(
    opensIntent: OpensAppIntent,
    dialog: IntentDialog
) -> Self where Self == IntentResultContainer, OpensAppIntent : AppIntent
```

## Parameters 

`opensIntent`  

An `AppIntent` to shows the result of current intent

`dialog`  

A custom success dialog

