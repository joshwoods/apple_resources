

- Security
-  SecTransformExecuteAsync(\_:\_:\_:) Deprecated

Function

# SecTransformExecuteAsync(\_:\_:\_:)

Executes transform or transform group asynchronously.

macOS 10.7–12.0Deprecated

``` source
func SecTransformExecuteAsync(
    _ transformRef: SecTransform,
    _ deliveryQueue: dispatch_queue_t,
    _ deliveryBlock: @escaping SecMessageBlock
)
```

Deprecated

SecTransform is no longer supported

## Parameters 

`transformRef`  

The transform to execute.

`deliveryQueue`  

A dispatch queue on which to deliver the results of this transform.

`deliveryBlock`  

A SecMessageBlock to asynchronously receive the results of the transform.

## Discussion

SecTransformExecuteAsync works just like the SecTransformExecute API except that it returns results to the deliveryBlock. There may be multple results depending on the transform. The block knows that the processing is complete when the isFinal parameter is set to true. If an error occurs the block’s error parameter is set and the isFinal parameter will be set to true.

