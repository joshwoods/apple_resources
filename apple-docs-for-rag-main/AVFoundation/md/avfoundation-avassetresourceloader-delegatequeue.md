

- AVFoundation
- AVAssetResourceLoader
-  delegateQueue 

Instance Property

# delegateQueue

The dispatch queue to use when handling resource requests.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
var delegateQueue: dispatch_queue_t? { get }
```

## Discussion

Resource requests are processed synchronously on the specified dispatch queue.

## See Also

### Accessing the Delegate

func setDelegate((any AVAssetResourceLoaderDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue to use with the resource loader.

var delegate: (any AVAssetResourceLoaderDelegate)?

The delegate object to use when handling resource requests.

protocol AVAssetResourceLoaderDelegate

Methods you can implement to handle resource-loading requests coming from a URL asset.

