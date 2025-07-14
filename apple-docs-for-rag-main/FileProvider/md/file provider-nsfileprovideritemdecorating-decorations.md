

- File Provider
- NSFileProviderItemDecorating
-  decorations 

Instance Property

# decorations

Asks the item for an array of decorations.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
var decorations: [NSFileProviderItemDecorationIdentifier]? { get }
```

**Required**

## Discussion

The system calls this method to request the item’s decorations. Your implementation should return an array of NSFileProviderItemDecorationIdentifier instances.

