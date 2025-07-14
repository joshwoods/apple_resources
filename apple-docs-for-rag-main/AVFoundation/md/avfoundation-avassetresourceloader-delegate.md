

- AVFoundation
- AVAssetResourceLoader
-  delegate 

Instance Property

# delegate

The delegate object to use when handling resource requests.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+

``` source
weak var delegate: (any AVAssetResourceLoaderDelegate)? { get }
```

## Discussion

The delegate object is responsible for indicating whether or not it is able to handle a resource request. And for those requests it does handle, the delegate object must initiate the loading of the requested resource.

## See Also

### Accessing the Delegate

func setDelegate((any AVAssetResourceLoaderDelegate)?, queue: dispatch_queue_t?)

Sets the delegate and dispatch queue to use with the resource loader.

protocol AVAssetResourceLoaderDelegate

Methods you can implement to handle resource-loading requests coming from a URL asset.

var delegateQueue: dispatch_queue_t?

The dispatch queue to use when handling resource requests.

