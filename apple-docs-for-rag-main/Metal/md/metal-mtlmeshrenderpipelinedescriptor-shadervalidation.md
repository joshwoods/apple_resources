

- Metal
- MTLMeshRenderPipelineDescriptor
-  shaderValidation 

Instance Property

# shaderValidation

A value that enables or disables shader validation for the pipeline.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+

``` source
var shaderValidation: MTLShaderValidation { get set }
```

## Discussion

You can override the value using either of these environment variables: `MTL_SHADER_VALIDATION_ENABLE_PIPELINES` or `MTL_SHADER_VALIDATION_DISABLE_PIPELINES.`

