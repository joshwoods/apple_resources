

- AppKit
- NSDraggingImageComponent
-  key 

Instance Property

# key

The unique name of this image component instance.

macOS 10.7+

``` source
var key: NSDraggingItem.ImageComponentKey { get set }
```

## Discussion

The key must be unique for each component in an NSDraggingItem instance. You can create your own named components, however the keys described in NSDragImage Component Keys have special meanings.

When an NSDraggingItem instances imageComponents are changed by one of the `enumerateDraggingItemsWithOptions:forView:classes:searchOptions:usingBlock:` methods the image associated with this key is morphed into the new image component’s image associated with the same key.

