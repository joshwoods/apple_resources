

- Metal
-  MTLNewComputePipelineStateCompletionHandler 

Type Alias

# MTLNewComputePipelineStateCompletionHandler

A completion handler signature a method calls when it finishes creating a compute pipeline.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
typealias MTLNewComputePipelineStateCompletionHandler = ((any MTLComputePipelineState)?, (any Error)?) -> Void
```

## Parameters 

`computePipelineState`  

An MTLComputePipelineState instance if the method completes successfully; otherwise `nil`.

`error`  

On return, if an error occurs, a pointer to an error information instance; otherwise `nil`.

## See Also

### Supporting Types

typealias MTLNewRenderPipelineStateCompletionHandler

A completion handler signature a method calls when it finishes creating a render pipeline.

typealias MTLNewRenderPipelineStateWithReflectionCompletionHandler

A completion handler signature a method calls when it finishes creating a render pipeline and reflection information.

typealias MTLNewComputePipelineStateWithReflectionCompletionHandler

A completion handler signature a method calls when it finishes creating a compute pipeline and reflection information.

