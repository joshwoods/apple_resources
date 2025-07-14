

- Model I/O
-  MDLMaterialPropertyNode 

Class

# MDLMaterialPropertyNode

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MDLMaterialPropertyNode
```

## Topics

### Initializers

init(inputs: [MDLMaterialProperty], outputs: [MDLMaterialProperty], evaluationFunction: (MDLMaterialPropertyNode) -> Void)

### Instance Properties

var evaluationFunction: (MDLMaterialPropertyNode) -> Void

var inputs: [MDLMaterialProperty]

var outputs: [MDLMaterialProperty]

## Relationships

### Inherits From

- NSObject

### Inherited By

- MDLMaterialPropertyGraph

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- MDLNamed
- NSObjectProtocol

## See Also

### Materials

class MDLMaterial

A collection of material properties that together describe the intended surface appearance for rendering a 3D object.

class MDLMaterialProperty

A definition for one specific aspect of the rendering parameters for a material.

class MDLMaterialPropertyConnection

class MDLMaterialPropertyGraph

class MDLScatteringFunction

A set of material properties that describes a basic shading model for materials, and the superclass for more complex shading models.

class MDLPhysicallyPlausibleScatteringFunction

A set of material properties that describes a physically realistic shading model for materials.

