

- RealityKit
- ResolvedModel3D
-  resizable(\_:) 

Instance Method

# resizable(\_:)

Allows this model to resize itself to fit its container.

RealityKitSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
func resizable(_ isResizable: Bool = true) -> ResolvedModel3D
```

## Discussion

Note

By default, `Model3D` sizes itself based on the intrinsic size of the underlying model file. Setting this will scale the model to fit its container instead. To preserve the intrinsic aspect ratio of the model, use doc://com.apple.documentation/documentationSwiftUI/View/aspectRatio(\_:contentMode:).

