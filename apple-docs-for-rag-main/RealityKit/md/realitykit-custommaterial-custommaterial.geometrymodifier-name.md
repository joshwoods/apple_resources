

- RealityKit
- CustomMaterial
- CustomMaterial.GeometryModifier
-  name 

Instance Property

# name

The name of the geometry modifier function.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+

``` source
var name: String
```

## Discussion

This is the name of the Metal function that the custom material uses as its geometry modifier. The name needs to match the name of a Metal function in your Xcode project without parameters or parentheses.

## See Also

### Accessing geometry modifier properties

var library: any MTLLibrary

The Metal library that contains this surface shader function.

