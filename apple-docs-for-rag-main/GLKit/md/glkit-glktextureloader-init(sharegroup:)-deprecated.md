

- GLKit
- GLKTextureLoader
-  init(sharegroup:) Deprecated

Initializer

# init(sharegroup:)

Initializes a new texture loader object.

iOS 5.0–12.0DeprecatediPadOS 5.0–12.0DeprecatedtvOS 9.0–12.0Deprecated

``` source
init(sharegroup: EAGLSharegroup)
```

Deprecated

OpenGLES API deprecated. (Define GLES_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`sharegroup`  

The sharegroup used to store new textures.

## Return Value

A newly initialized texture loader.

## Discussion

You only create a texture loader object when your app needs to load textures asynchronously.

## See Also

### Initialization

init(share: NSOpenGLContext)

Initializes a new texture loader object.

Deprecated

