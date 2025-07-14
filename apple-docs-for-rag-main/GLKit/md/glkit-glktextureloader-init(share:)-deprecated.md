

- GLKit
- GLKTextureLoader
-  init(share:) Deprecated

Initializer

# init(share:)

Initializes a new texture loader object.

macOS 10.8–10.14Deprecated

``` source
init(share context: NSOpenGLContext)
```

Deprecated

OpenGL API deprecated. (Define GL_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`context`  

The share context used to store new textures.

## Return Value

A newly initialized texture loader.

## Discussion

You only create a texture loader object when your app needs to load textures asynchronously.

## See Also

### Initialization

init(sharegroup: EAGLSharegroup)

Initializes a new texture loader object.

Deprecated

