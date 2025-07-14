

- RealityKit
- RealityViewContent
- RealityViewContent.Body
-  upperLimbVisibility(\_:) 

Instance Method

# upperLimbVisibility(\_:)

Sets the preferred visibility of the user’s upper limbs, while an `ImmersiveSpace` scene is presented.

RealityKitSwiftUIvisionOS 1.0+

``` source
nonisolated
func upperLimbVisibility(_ preferredVisibility: Visibility) -> some View
```

## Discussion

The system can show the user’s upper limbs during fully immersive experiences, but you can also hide them, for example, in order to display virtual hands instead.

Note that this modifier only sets a preference and ultimately the system will decide if it will honor it or not. The system may by unable to honor the preference if the immersive space is currently not visible.

