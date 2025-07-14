

- RealityKit
- ResolvedModel3D
-  fileDialogDefaultDirectory(\_:) 

Instance Method

# fileDialogDefaultDirectory(\_:)

Configures the `fileExporter`, `fileImporter`, or `fileMover` to open with the specified default directory.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+visionOS

``` source
nonisolated
func fileDialogDefaultDirectory(_ defaultDirectory: URL?) -> some View
```

## Parameters 

`defaultDirectory`  

The directory to show when the system file dialog launches. If the given file dialog has a `fileDialogCustomizationID` if stores the user-chosen directory and subsequently opens with it, ignoring the default value provided in this modifier.

