

- Foundation
- NSCache
-  evictsObjectsWithDiscardedContent 

Instance Property

# evictsObjectsWithDiscardedContent

Whether the cache will automatically evict discardable-content objects whose content has been discarded.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var evictsObjectsWithDiscardedContent: Bool { get set }
```

## Discussion

If true, the cache will evict a discardable-content object after its content is discarded. If false, it will not. The default value is true.

## See Also

### Managing Discardable Content

protocol NSDiscardableContent

You implement this protocol when a class’s objects have subcomponents that can be discarded when not being used, thereby giving an application a smaller memory footprint.

