

- Metal
- MTLDrawable
-  drawableID 

Instance Property

# drawableID

A positive integer that identifies the drawable.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.4+macOS 10.15.4+tvOS 10.2+visionOS 1.0+

``` source
var drawableID: Int { get }
```

**Required**

## Discussion

Drawable objects are usually owned by some other object, such as a CAMetalLayer. The owning object gives the first drawable it creates an ID of `0`, and it increments the ID by `1` for each additional drawable it creates.

