

- Metal
-  MTLNewRenderPipelineStateWithReflectionCompletionHandler 

Type Alias

# MTLNewRenderPipelineStateWithReflectionCompletionHandler

A completion handler signature a method calls when it finishes creating a render pipeline and reflection information.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MTLNewRenderPipelineStateWithReflectionCompletionHandler = ((any MTLRenderPipelineState)?, MTLRenderPipelineReflection?, (any Error)?) -> Void
```

## Parameters 

`renderPipelineState`  

An MTLRenderPipelineState instance if the method successfully compiles the library without any errors; otherwise `nil`.

`reflection`  

An MTLRenderPipelineReflection instance if the method completes successfully; otherwise `nil`.

`error`  

If an error occurs, an error information instance; otherwise `nil`.

## See Also

### Supporting Types

typealias MTLNewRenderPipelineStateCompletionHandler

A completion handler signature a method calls when it finishes creating a render pipeline.

typealias MTLNewComputePipelineStateCompletionHandler

A completion handler signature a method calls when it finishes creating a compute pipeline.

typealias MTLNewComputePipelineStateWithReflectionCompletionHandler

A completion handler signature a method calls when it finishes creating a compute pipeline and reflection information.

