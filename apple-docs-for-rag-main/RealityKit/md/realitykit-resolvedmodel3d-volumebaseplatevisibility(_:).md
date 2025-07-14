

- RealityKit
- ResolvedModel3D
-  volumeBaseplateVisibility(\_:) 

Instance Method

# volumeBaseplateVisibility(\_:)

Sets the visibility of the baseplate of a volume, which appears when a user looks towards the ‘floor’ of a volume and during resize. Both `automatic` and `visible` will show the baseplate. `hidden` will never show it.

RealityKitSwiftUIvisionOS 2.0+

``` source
nonisolated
func volumeBaseplateVisibility(_ visibility: Visibility) -> some View
```

## Discussion

The baseplate is a semi-transparent view that appears on the ‘floor’ of a volume.

Usage:

```
WindowGroup() {
    Poker()
        .volumeBaseplateVisibility(.visible)
}
.windowStyle(.volumetric)
```

Defaults to `automatic` (visible).

