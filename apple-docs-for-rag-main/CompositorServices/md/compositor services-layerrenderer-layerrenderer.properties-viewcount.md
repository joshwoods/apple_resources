

- Compositor Services
- LayerRenderer
- LayerRenderer.Properties
-  viewCount 

Instance Property

# viewCount

The number of views that you must fill with content.

visionOS 1.0+

``` source
var viewCount: Int { get }
```

## Discussion

This property tells you how many views you’re responsible for filling with your content. For example, this function returns `1` for a monoscopic display and `2` for a stereoscopic display.

