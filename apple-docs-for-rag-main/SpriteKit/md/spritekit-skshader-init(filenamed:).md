

- SpriteKit
- SKShader
-  init(fileNamed:) 

Initializer

# init(fileNamed:)

Creates a new shader object by loading the source for a fragment shader from a file stored in the app’s bundle.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
convenience init(fileNamed name: String)
```

## Parameters 

`name`  

The name of the fragment shader to load. The file must be present in your app bundle with the same name and a `.fsh` file extension.

## Return Value

A newly initialized shader object whose initial source is loaded from the shader file.

## See Also

### Creating a Shader

Creating a Custom Fragment Shader

Write a fragment shader using the set of SpriteKit-exposed symbols, and supply it with custom data.

init(source: String, uniforms: [SKUniform])

Initializes a new shader object using the specified source and uniform data.

init(source: String)

Initializes a new shader object using the specified source code.

