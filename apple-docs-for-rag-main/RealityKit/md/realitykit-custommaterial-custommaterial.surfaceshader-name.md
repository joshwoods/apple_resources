

- RealityKit
- CustomMaterial
- CustomMaterial.SurfaceShader
-  name 

Instance Property

# name

The name of the surface shader function.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var name: String
```

## Discussion

This is the name of the Metal function the custom material uses as its surface shader. The name needs to match the name of a Metal function in your Xcode project and can’t include parameters or parentheses.

## See Also

### Accessing surface shader properties

var library: any MTLLibrary

The Metal library that contains this surface shader function.

