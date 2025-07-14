

- Core Foundation
- CGRect
-  clip() 

Instance Method

# clip()

Modifies the current graphics context clipping path by intersecting it with this rect. This permanently modifies the graphics state, so the current state should be saved beforehand and restored afterwards.

macOS 10.9+Swift 4.0+

``` source
func clip()
```

## Discussion

Precondition

There must be a set current NSGraphicsContext.

