

- Cinematic
- CNScript
-  fNumber 

Instance Property

# fNumber

The f-stop value which inversely affects the aperture used to render the Cinematic image.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final var fNumber: Float { get set }
```

## Discussion

Pass this to the rendering session in the rendering frame attributes to match the selected aperture. Change this property when the user selects a different aperture for the edited movie. Reflect script changes for later restoration by making changes to this property.

