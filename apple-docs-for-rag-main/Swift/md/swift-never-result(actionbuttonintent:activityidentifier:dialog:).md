

- Swift
- Never
-  result(actionButtonIntent:activityIdentifier:dialog:) 

Type Method

# result(actionButtonIntent:activityIdentifier:dialog:)

Indicates the Intent finished performing with an `AppIntent` to continue with

SwiftAppIntentsiOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
static func result(
    actionButtonIntent: Intent,
    activityIdentifier: String,
    dialog: IntentDialog
) -> Self where Self == IntentResultContainer, Intent : AppIntent
```

## Parameters 

`dialog`  

A custom success dialog

