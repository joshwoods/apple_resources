

- GLKit
- GLKNamedEffect
-  prepareToDraw() 

Instance Method

# prepareToDraw()

Prepares an effect for OpenGL ES rendering.

iOS 5.0+iPadOS 5.0+macOS 10.8+tvOS 9.0+

``` source
func prepareToDraw()
```

**Required**

## Discussion

An effect binds a compiled shader program to the context and returns. Many effects also bind data to other OpenGL state variables—see the appropriate reference for each effect class.

