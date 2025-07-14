

- FamilyControls
- FamilyActivityTitleView
-  fileDialogMessage(\_:) 

Instance Method

# fileDialogMessage(\_:)

On macOS, configures the the `fileExporter`, `fileImporter`, or `fileMover` with a custom message that is presented to the user, similar to a title.

FamilyControlsSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+

``` source
nonisolated
func fileDialogMessage(_ message: S) -> some View where S : StringProtocol
```

## Parameters 

`message`  

The string to use as the file dialog message.

