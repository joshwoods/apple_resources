

- RealityKit
- UnlitMaterial
- UnlitMaterial.Program
- UnlitMaterial.Program.Descriptor
-  blendMode 

Instance Property

# blendMode

Modes that describe how materials using the created `UnlitMaterial.Program` will be blended with content behind them.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var blendMode: MaterialParameterTypes.BlendMode?
```

## Discussion

Default value is nil, which will cause this material to render opaque, and not blend with background content.

