

- SpriteKit
- SKUniform
-  uniformType 

Instance Property

# uniformType

The uniform object’s data type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var uniformType: SKUniformType { get }
```

## Discussion

A uniform object’s type is set to SKUniformType.none until the first time that the uniform variable’s value is set; this happens automatically if you use an initialization method that provides an initial type and value. Once the uniform object is given an initial value, its type changes to that value’s type and thereafter cannot be changed.

## See Also

### Reading Information About a Uniform

var name: String

The uniform’s name.

