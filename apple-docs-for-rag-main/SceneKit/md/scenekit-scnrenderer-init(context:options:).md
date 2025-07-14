

- SceneKit
- SCNRenderer
-  init(context:options:) 

Initializer

# init(context:options:)

Creates a renderer with the specified OpenGL context.

iOSiPadOSmacOStvOS

**macOS**

``` source
convenience init(
    context: CGLContextObj?,
    options: [AnyHashable : Any]? = nil
)
```

**iOS, iPadOS, tvOS**

``` source
convenience init(
    context: EAGLContext?,
    options: [AnyHashable : Any]? = nil
)
```

## Parameters 

`context`  

An OpenGL rendering context: either a cglContextObj reference (in macOS) or an EAGLContext object (in iOS).

`options`  

An optional dictionary for future extensions.

## Return Value

A new renderer object.

## Discussion

Use this initializer to create a SceneKit renderer that draws into OpenGL context your app already uses to draw other content. To tell SceneKit to render your content, call the SCNRenderer or SCNRenderer method.

## See Also

### Creating a Renderer

convenience init(device: (any MTLDevice)?, options: [AnyHashable : Any]?)

Creates a renderer with the specified Metal device.

