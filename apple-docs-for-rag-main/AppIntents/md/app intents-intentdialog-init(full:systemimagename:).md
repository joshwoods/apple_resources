

- App Intents
- IntentDialog
-  init(full:systemImageName:) 

Initializer

# init(full:systemImageName:)

The text you want the system to display, or speak, when requesting a value, asking for disambiguation, or confirming an action.

iOS 17.2+iPadOS 17.2+Mac Catalyst 17.2+macOS 14.2+tvOS 17.2+visionOS 1.0+watchOS 10.2+

``` source
init(
    full: LocalizedStringResource,
    systemImageName: String
)
```

## Discussion

Parameters:

- full: a standalone message that fully describes the output

- systemImageName: an SF Symbol that may be be used to represent the result

