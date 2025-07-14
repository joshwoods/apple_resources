

- Core Animation
- CAMetalLayer
-  allowsNextDrawableTimeout 

Instance Property

# allowsNextDrawableTimeout

A Boolean value that determines whether requests for a new buffer expire if the system can’t satisfy them.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var allowsNextDrawableTimeout: Bool { get set }
```

## Discussion

If true, the nextDrawable() method returns nil if it can’t provide a drawable object within one second. If false, the nextDrawable() method waits indefinitely for a drawable to become available.

The default value is true.

## See Also

### Obtaining a Metal Drawable

func nextDrawable() -> (any CAMetalDrawable)?

Waits until a Metal drawable is available, and then returns it.

var maximumDrawableCount: Int

The number of Metal drawables in the resource pool managed by Core Animation.

