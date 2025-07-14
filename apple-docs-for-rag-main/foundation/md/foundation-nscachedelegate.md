

- Foundation
-  NSCacheDelegate 

Protocol

# NSCacheDelegate

The delegate of an NSCache object implements this protocol to perform specialized actions when an object is about to be evicted or removed from the cache.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSCacheDelegate : NSObjectProtocol
```

## Topics

### Responding to Object Eviction

func cache(NSCache&lt;AnyObject, AnyObject>, willEvictObject: Any)

Called when an object is about to be evicted or removed from the cache.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Managing the Delegate

var delegate: (any NSCacheDelegate)?

The cache’s delegate.

