

- MusicKit
- ArtworkImage
-  fileDialogDefaultDirectory(\_:) 

Instance Method

# fileDialogDefaultDirectory(\_:)

Configures the `fileExporter`, `fileImporter`, or `fileMover` to open with the specified default directory.

MusicKitSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func fileDialogDefaultDirectory(_ defaultDirectory: URL?) -> some View
```

## Parameters 

`defaultDirectory`  

The directory to show when the system file dialog launches. If the given file dialog has a `fileDialogCustomizationID` if stores the user-chosen directory and subsequently opens with it, ignoring the default value provided in this modifier.

