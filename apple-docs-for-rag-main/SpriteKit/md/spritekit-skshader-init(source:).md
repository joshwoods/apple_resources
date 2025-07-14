

- SpriteKit
- SKShader
-  init(source:) 

Initializer

# init(source:)

Initializes a new shader object using the specified source code.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
init(source: String)
```

## Parameters 

`source`  

A string that holds the initial source for the shader.

## Return Value

An initialized shader object.

## See Also

### Creating a Shader

Creating a Custom Fragment Shader

Write a fragment shader using the set of SpriteKit-exposed symbols, and supply it with custom data.

convenience init(fileNamed: String)

Creates a new shader object by loading the source for a fragment shader from a file stored in the app’s bundle.

init(source: String, uniforms: [SKUniform])

Initializes a new shader object using the specified source and uniform data.

