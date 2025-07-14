

- SwiftUI
- Material
-  materialActiveAppearance(\_:) 

Instance Method

# materialActiveAppearance(\_:)

Sets an explicit active appearance for this material.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
func materialActiveAppearance(_ appearance: MaterialActiveAppearance) -> Material
```

## Discussion

Materials used as the `window` container background on macOS will automatically appear inactive when their the window appears inactive, but can be made to always appear active by setting the active appearance behavior to be always active:

```
Text("Hello, World!")
    .containerBackground(
        Material.regular.materialActiveAppearance(.active),
        for: .window)
```

