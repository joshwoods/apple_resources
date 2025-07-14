

- Core Animation
- CAMetalLayer
-  maximumDrawableCount 

Instance Property

# maximumDrawableCount

The number of Metal drawables in the resource pool managed by Core Animation.

iOS 11.2+iPadOS 11.2+Mac Catalyst 13.1+macOS 10.13.2+tvOS 11.2+visionOS 1.0+

``` source
var maximumDrawableCount: Int { get set }
```

## Discussion

You can set this value to `2` or `3` only; if you pass a different value, Core Animation ignores the value and throws an exception.

The default value is `3`.

## See Also

### Obtaining a Metal Drawable

func nextDrawable() -> (any CAMetalDrawable)?

Waits until a Metal drawable is available, and then returns it.

var allowsNextDrawableTimeout: Bool

A Boolean value that determines whether requests for a new buffer expire if the system can’t satisfy them.

