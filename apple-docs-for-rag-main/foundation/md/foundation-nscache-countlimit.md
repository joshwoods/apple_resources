

- Foundation
- NSCache
-  countLimit 

Instance Property

# countLimit

The maximum number of objects the cache should hold.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var countLimit: Int { get set }
```

## Discussion

If `0`, there is no count limit. The default value is `0`.

This is not a strict limit—if the cache goes over the limit, an object in the cache could be evicted instantly, later, or possibly never, depending on the implementation details of the cache.

## See Also

### Managing Cache Size

var totalCostLimit: Int

The maximum total cost that the cache can hold before it starts evicting objects.

