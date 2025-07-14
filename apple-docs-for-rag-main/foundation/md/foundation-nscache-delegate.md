

- Foundation
- NSCache
-  delegate 

Instance Property

# delegate

The cache’s delegate.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
unowned(unsafe) var delegate: (any NSCacheDelegate)? { get set }
```

## Discussion

The delegate must adopt the NSCacheDelegate protocol.

## See Also

### Managing the Delegate

protocol NSCacheDelegate

The delegate of an NSCache object implements this protocol to perform specialized actions when an object is about to be evicted or removed from the cache.

