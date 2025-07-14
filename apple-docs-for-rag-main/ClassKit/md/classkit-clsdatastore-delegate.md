

- ClassKit
- CLSDataStore
-  delegate 

Instance Property

# delegate

The data store delegate instance.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
weak var delegate: (any CLSDataStoreDelegate)? { get set }
```

## Discussion

The data store delegate creates contexts when the data store receives a request for a context it doesn’t already have. The data store calls on its delegate to build the missing context.

For privacy reasons, and depending on factors like the user’s role as student, teacher, or unmanaged user, the data store may or may not keep a persistent copy of a context returned by the delegate. As a result, it’s impossible to predict from within your app which context requests might result in a delegate callback. So you should be prepared for any context request that you make of the data store to result in a delegate callback.

## See Also

### Managing the delegate

Building missing contexts

Create and initialize missing contexts.

protocol CLSDataStoreDelegate

An interface the data store uses to request new contexts.

