

- Model I/O
-  MDLMaterialPropertyGraph 

Class

# MDLMaterialPropertyGraph

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class MDLMaterialPropertyGraph
```

## Topics

### Initializers

init(nodes: [MDLMaterialPropertyNode], connections: [MDLMaterialPropertyConnection])

### Instance Properties

var connections: [MDLMaterialPropertyConnection]

var nodes: [MDLMaterialPropertyNode]

### Instance Methods

func evaluate()

## Relationships

### Inherits From

- MDLMaterialPropertyNode

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

class MDLMaterialPropertyNode

class MDLScatteringFunction

A set of material properties that describes a basic shading model for materials, and the superclass for more complex shading models.

class MDLPhysicallyPlausibleScatteringFunction

A set of material properties that describes a physically realistic shading model for materials.

