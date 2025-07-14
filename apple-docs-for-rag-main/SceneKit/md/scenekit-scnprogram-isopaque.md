

- SceneKit
- SCNProgram
-  isOpaque 

Instance Property

# isOpaque

A Boolean value that indicates whether fragments rendered by the program are fully opaque.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOS

``` source
var isOpaque: Bool { get set }
```

## Discussion

The default value is true, indicating that all fragments rendered by the program are fully opaque. In this case, SceneKit can composite these fragments into the final image without blending, improving rendering performance.

If your shader program renders fragment colors whose alpha value is less than `1.0`, change this property’s value to false for proper blending.

