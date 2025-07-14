

- Foundation
- NSFileAccessIntent
-  url 

Instance Property

# url

The current URL for the item managed by the file access intent instance. (read-only)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var url: URL { get }
```

## Discussion

Always use the URL returned by this property inside the accessor block of a file coordinator’s coordinate(with:queue:byAccessor:) method. This property’s value may be different from the original URL, because the item was either moved or renamed while the file coordinator waited for access.

## See Also

### Related Documentation

func coordinate(with: [NSFileAccessIntent], queue: OperationQueue, byAccessor: ((any Error)?) -> Void)

Performs a number of coordinated-read or -write operations asynchronously.

