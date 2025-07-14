

- SceneKit
- SCNRenderer
-  render() Deprecated

Instance Method

# render()

Renders the scene’s contents in the renderer’s OpenGL context.

iOS 8.0–9.0DeprecatediPadOS 8.0–9.0DeprecatedmacOS 10.8–10.11Deprecated

``` source
func render()
```

## Discussion

This method can be used only with an SCNRenderer object created with the SCNRenderer initializer. Call this method to tell SceneKit to draw the renderer’s scene into the OpenGL context you created the renderer with.

When you call this method, SceneKit updates its hierarchy of presentation nodes based on the current system time, and then draws the scene.

## See Also

### Rendering a Scene Using OpenGL

func render(atTime: CFTimeInterval)

Renders the scene’s contents at the specified system time in the renderer’s OpenGL context.

