

- SpriteKit
- SKTexture
-  applying(\_:) 

Instance Method

# applying(\_:)

Creates a new texture by applying a Core Image filter to an existing texture.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
func applying(_ filter: CIFilter) -> Self
```

## Parameters 

`filter`  

A Core Image filter that requires a single `inputImage` parameter and produces an `outputImage` parameter.

## Return Value

A new texture object.

## Discussion

The image data is copied before control is returned to your game.

