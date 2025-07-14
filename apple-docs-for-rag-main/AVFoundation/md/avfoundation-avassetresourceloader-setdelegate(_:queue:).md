

- AVFoundation
- AVAssetResourceLoader
-  setDelegate(\_:queue:) 

Instance Method

# setDelegate(\_:queue:)

Sets the delegate and dispatch queue to use with the resource loader.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
func setDelegate(
    _ delegate: (any AVAssetResourceLoaderDelegate)?,
    queue delegateQueue: dispatch_queue_t?
)
```

## Parameters 

`delegate`  

The delegate object to query when handling resource requests. You may specify `nil` if you want to clear the delegate object. The resource loader does not store a strong reference to the delegate object.

`delegateQueue`  

The dispatch queue on which to execute resource requests. If the `delegate` parameter is not `nil`, this parameter must also not be `nil` and must contain a valid dispatch queue. However, if `delegate` is `nil`, this parameter may also be `nil`.

The resource loader maintains a strong reference to the dispatch queue you specify.

## Discussion

You use this method to specify the object to use when handling resource requests and the dispatch queue on which to process those requests. Resource requests are processed synchronously on the dispatch queue you provide.

## See Also

### Accessing the Delegate

var delegate: (any AVAssetResourceLoaderDelegate)?

The delegate object to use when handling resource requests.

protocol AVAssetResourceLoaderDelegate

Methods you can implement to handle resource-loading requests coming from a URL asset.

var delegateQueue: dispatch_queue_t?

The dispatch queue to use when handling resource requests.

