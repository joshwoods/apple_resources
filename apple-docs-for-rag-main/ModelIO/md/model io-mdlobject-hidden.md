

- Model I/O
- MDLObject
-  hidden 

Instance Property

# hidden

A Boolean value indicating whether this object should be used in rendering.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var hidden: Bool { get set }
```

## Discussion

Model I/O is not a renderer, so this property is purely informational.

Renderers using assets imported using Model I/O can use this property to determine whether to include meshes in a rendered scene, apply lighting from light sources, and so on.

## See Also

### Managing Rendering Intent

var instance: MDLObject?

The primary object, if applicable, of which this object is an instance.

var path: String

A path that identifies the object in an asset’s object hierarchy using object names.

var components: [any MDLComponent]

