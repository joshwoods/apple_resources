

- Metal
- MTLRenderPipelineReflection
-  objectBindings 

Instance Property

# objectBindings

An array of binding instances, each of which represents a parameter of the pipeline state’s object shader.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
var objectBindings: [any MTLBinding] { get }
```

## Discussion

The MTLBinding elements in the array are in the same order as the object shader’s declaration signature.

## See Also

### Inspecting a Shader’s Parameter

var fragmentBindings: [any MTLBinding]

An array of binding instances, each of which represents a parameter of the pipeline state’s fragment shader.

var meshBindings: [any MTLBinding]

An array of binding instances, each of which represents a parameter of the pipeline state’s mesh shader.

var tileBindings: [any MTLBinding]

An array of binding instances, each of which represents a parameter of the pipeline state’s tile shader.

var vertexBindings: [any MTLBinding]

An array of binding instances, each of which represents a parameter of the pipeline state’s vertex shader.

