

- Core Animation
- CAEAGLLayer
-  presentsWithTransaction Deprecated

Instance Property

# presentsWithTransaction

A Boolean value that determines whether the layer presents its content using a Core Animation transaction.

iOS 9.0–12.0DeprecatediPadOS 9.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
var presentsWithTransaction: Bool { get set }
```

## Discussion

By default this value is false: CAEAGLLayer displays the output of a rendering pass to the display as quickly as possible and asynchronously to any Core Animation transactions. However, if your game or app combines OpenGL and Core Animation content, it’s not guaranteed that your OpenGL content will arrive in the same frame as your Core Animation content. This could be an issue if, for example, your app draws UIKit content (such as labels with a target position and time) over the top of your CAEAGLLayer and the two domains need to be synchronized.

Setting this value to true changes this default behavior so that your CAEAGLLayer displays its drawable content synchronously, using whichever Core Animation transaction is current.

.

## See Also

### Accessing the Layer Properties

var drawableProperties: [String : Any]? { get set }

A dictionary of values that specify the desired characteristics of the drawable surface.

Deprecated

