

- App Intents
- SiriTipView
-  fileDialogConfirmationLabel(\_:) 

Instance Method

# fileDialogConfirmationLabel(\_:)

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with a custom confirmation button label.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func fileDialogConfirmationLabel(_ label: S) -> some View where S : StringProtocol
```

## Parameters 

`label`  

The string to use as the label for the confirmation button.

