

- Foundation
- URLCache
-  diskCapacity 

Instance Property

# diskCapacity

The capacity of the on-disk cache, in bytes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var diskCapacity: Int { get set }
```

## Mentioned in 

Accessing cached data

## Discussion

When set, the on-disk cache will truncate its contents to the given size, if necessary.

## See Also

### Getting and setting on-disk cache properties

var currentDiskUsage: Int

The current size of the on-disk cache, in bytes.

