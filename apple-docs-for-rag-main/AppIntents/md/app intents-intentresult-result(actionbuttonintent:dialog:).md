

- App Intents
- IntentResult
-  result(actionButtonIntent:dialog:) 

Type Method

# result(actionButtonIntent:dialog:)

Indicates the Intent finished performing with an `AppIntent` to continue with

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func result(
    actionButtonIntent: Intent,
    dialog: IntentDialog
) -> Self where Self == IntentResultContainer, Intent : AppIntent
```

## Parameters 

`dialog`  

A custom success dialog

