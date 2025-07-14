

- Foundation
- URLCache
-  memoryCapacity 

Instance Property

# memoryCapacity

The capacity of the in-memory cache, in bytes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.2+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var memoryCapacity: Int { get set }
```

## Mentioned in 

Accessing cached data

## Discussion

At the time this property is set, the in-memory cache will truncate its contents to the size given, if necessary.

## See Also

### Getting and setting in-memory cache properties

var currentMemoryUsage: Int

The current size of the in-memory cache, in bytes.

