

- SceneKit
- SCNWrapMode
-  SCNWrapMode.mirror 

Case

# SCNWrapMode.mirror

Texture sampling of texture coordinates outside range from `0.0` to `1.0` should behave as if the range reverses before repeating.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
case mirror
```

## Mentioned in 

SCNMirror

## Discussion

Texture sampling in areas of the material whose texture coordinates would fall outside from `0.0` to `1.0` results in tiling both texture image and its mirror image across the surface using the material.

## See Also

### Constants

case clamp

Texture coordinates are clamped to the range from `0.0` to `1.0`, inclusive.

case `repeat`

Texture sampling uses only the fractional part of texture coordinates, passing through the range from `0.0` to (but not including) `1.0`.

case clampToBorder

Texture sampling uses texture colors for coordinates in the range from `0.0` to `1.0` (inclusive) and the material property’s borderColor value otherwise.

SCNClamp

Equivalent to SCNWrapMode.clamp.

SCNRepeat

Equivalent to SCNWrapMode.repeat.

SCNClampToBorder

Equivalent to SCNWrapMode.clampToBorder.

SCNMirror

Equivalent to SCNWrapMode.mirror.

