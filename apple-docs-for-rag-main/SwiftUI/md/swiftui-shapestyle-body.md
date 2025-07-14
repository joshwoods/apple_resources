

- SwiftUI
- ShapeStyle
-  body 

Instance Property

# body

A rectangular view that’s filled with the shape style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var body: _ShapeView { get }
```

Available when `Self` conforms to `View` and `Body` is `_ShapeView`.

## Discussion

For a ShapeStyle that also conforms to the View protocol, like Color or LinearGradient, this default implementation of the body property provides a visual representation for the shape style. As a result, you can use the shape style in a view hierarchy like any other view:

```
ZStack {
    Color.cyan
    Text("Hello!")
}
.frame(width: 200, height: 50)
```

