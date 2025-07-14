

- RealityKit
- UnlitMaterial
- UnlitMaterial.Program
- UnlitMaterial.Program.Descriptor
-  applyPostProcessToneMap 

Instance Property

# applyPostProcessToneMap

A Boolean value that determines whether RealityKit will tonemap the output of this material.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var applyPostProcessToneMap: Bool
```

## Discussion

If true, the created `UnlitMaterial.Program` will tonemap its color output to better match the rest of the scene; if false, the created `UnlitMaterial.Program` will output its color without modification.

Default value is true.

