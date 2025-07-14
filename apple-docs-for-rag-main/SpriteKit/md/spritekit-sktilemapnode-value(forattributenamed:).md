

- SpriteKit
- SKTileMapNode
-  value(forAttributeNamed:) 

Instance Method

# value(forAttributeNamed:)

The value of a shader attribute.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func value(forAttributeNamed key: String) -> SKAttributeValue?
```

**watchOS**

``` source
func value(forAttributeNamed key: String) -> SKAttributeValue?
```

## Parameters 

`key`  

The attribute name.

## Return Value

An attribute value object containing the scalar or vector value or `nil` if no such attribute exists.

## See Also

### Working with Custom Shaders

var shader: SKShader?

Defines a shader which is applied to each tile of the tile map.

var attributeValues: [String : SKAttributeValue]

The values of each attribute associated with the node’s attached shader.

func setValue(SKAttributeValue, forAttribute: String)

Sets an attribute value for an attached shader.

