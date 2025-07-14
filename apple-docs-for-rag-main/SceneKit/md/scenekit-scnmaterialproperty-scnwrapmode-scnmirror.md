

- SceneKit
- SCNMaterialProperty
- SCNWrapMode
-  SCNMirror 

Article

# SCNMirror

Equivalent to SCNWrapMode.mirror.

## Overview

Deprecated in OS X v10.9. Use SCNWrapMode.mirror instead.

## See Also

### Constants

case clamp

Texture coordinates are clamped to the range from `0.0` to `1.0`, inclusive.

case `repeat`

Texture sampling uses only the fractional part of texture coordinates, passing through the range from `0.0` to (but not including) `1.0`.

case clampToBorder

Texture sampling uses texture colors for coordinates in the range from `0.0` to `1.0` (inclusive) and the material property’s borderColor value otherwise.

case mirror

Texture sampling of texture coordinates outside range from `0.0` to `1.0` should behave as if the range reverses before repeating.

SCNClamp

Equivalent to SCNWrapMode.clamp.

SCNRepeat

Equivalent to SCNWrapMode.repeat.

SCNClampToBorder

Equivalent to SCNWrapMode.clampToBorder.

