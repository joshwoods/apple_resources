

- Metal
-  MTLNewRenderPipelineStateCompletionHandler 

Type Alias

# MTLNewRenderPipelineStateCompletionHandler

A completion handler signature a method calls when it finishes creating a render pipeline.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MTLNewRenderPipelineStateCompletionHandler = ((any MTLRenderPipelineState)?, (any Error)?) -> Void
```

## Parameters 

`renderPipelineState`  

An MTLRenderPipelineState instance if the method completes successfully; otherwise `nil`.

`error`  

If an error occurs, an error information instance; otherwise `nil`.

## See Also

### Supporting Types

typealias MTLNewRenderPipelineStateWithReflectionCompletionHandler

A completion handler signature a method calls when it finishes creating a render pipeline and reflection information.

typealias MTLNewComputePipelineStateCompletionHandler

A completion handler signature a method calls when it finishes creating a compute pipeline.

typealias MTLNewComputePipelineStateWithReflectionCompletionHandler

A completion handler signature a method calls when it finishes creating a compute pipeline and reflection information.

