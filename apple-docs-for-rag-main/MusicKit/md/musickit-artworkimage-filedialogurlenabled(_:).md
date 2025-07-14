

- MusicKit
- ArtworkImage
-  fileDialogURLEnabled(\_:) 

Instance Method

# fileDialogURLEnabled(\_:)

On macOS, configures the the `fileImporter` or `fileMover` to conditionally disable presented URLs.

MusicKitSwiftUIiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
nonisolated
func fileDialogURLEnabled(_ predicate: Predicate) -> some View
```

## Parameters 

`predicate`  

The predicate that evaluates the URLs presented to the user to conditionally disable them. The implementation is expected to have constant complexity and should not access the files contents or metadata. A common use case is inspecting the path or the file name.

