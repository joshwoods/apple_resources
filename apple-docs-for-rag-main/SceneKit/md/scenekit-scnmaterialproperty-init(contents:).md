

- SceneKit
- SCNMaterialProperty
-  init(contents:) 

Initializer

# init(contents:)

Creates a new material property object with the specified contents.

iOSiPadOSMac Catalyst 13.1+macOS 10.9+tvOSvisionOSwatchOS

``` source
convenience init(contents: Any)
```

## Parameters 

`contents`  

The visual contents of the material property—a color, image, or source of animated content. For details, see the discussion of the contents property.

## Return Value

A new material property object.

## Discussion

Newly created SCNMaterial objects contain SCNMaterialProperty instances for all of their visual properties. To change a material’s visual properties, you modify those instances rather than creating new material property objects.

You create new SCNMaterialProperty instances to provide textures for use with custom GLSL shaders—for details, see SCNShadable.

