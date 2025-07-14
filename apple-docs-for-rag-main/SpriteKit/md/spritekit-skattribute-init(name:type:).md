

- SpriteKit
- SKAttribute
-  init(name:type:) 

Initializer

# init(name:type:)

Creates and initializes a new attribute object of a specified type with a name that can be referenced within the shader.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    name: String,
    type: SKAttributeType
)
```

## Parameters 

`name`  

The name of the attribute.

`type`  

The type of the attribute.

## Return Value

A new attribute object.

## Discussion

Attribute names are typically named with a preceding “a” and an underscore. The following code shows how to initialize an attribute named `a_frequency` which is of type SKAttributeType.float.

```
let attribute = SKAttribute(name: "a_frequency", 
                            type: SKAttributeType.float)
```

