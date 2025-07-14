

- SwiftUI
- Layout
-  Cache 

Associated Type

# Cache

Cached values associated with the layout instance.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
associatedtype Cache = Void
```

**Required**

## Discussion

If you create a cache for your custom layout, you can use a type alias to define this type as your data storage type. Alternatively, you can refer to the data storage type directly in all the places where you work with the cache.

See makeCache(subviews:) for more information.

## See Also

### Managing a cache

func makeCache(subviews: Self.Subviews) -> Self.Cache

Creates and initializes a cache for a layout instance.

**Required** Default implementation provided.

func updateCache(inout Self.Cache, subviews: Self.Subviews)

Updates the layout’s cache when something changes.

**Required** Default implementation provided.

