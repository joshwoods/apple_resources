

- Core Animation
- CAMetalDrawable
-  layer 

Instance Property

# layer

The layer that owns this drawable object.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var layer: CAMetalLayer { get }
```

**Required**

## Discussion

When you present the drawable object, it becomes the owning layer’s content.

