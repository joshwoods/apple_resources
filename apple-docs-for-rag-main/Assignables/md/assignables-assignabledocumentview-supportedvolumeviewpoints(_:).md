

- Assignables
- AssignableDocumentView
-  supportedVolumeViewpoints(\_:) 

Instance Method

# supportedVolumeViewpoints(\_:)

Specifies which viewpoints are supported for the window bar and ornaments in a volume.

AssignablesSwiftUIvisionOS 2.0+

``` source
nonisolated
func supportedVolumeViewpoints(_ viewpoints: SquareAzimuth.Set) -> some View
```

## Discussion

This defaults to all viewpoints and determines which viewpoints the window bar and ornaments will ‘follow’ the user to as they move around the volume.

