

- RealityKit
- ARView
- ARView.DebugOptions
-  ARView.DebugOptions.ArrayLiteralElement 

Type Alias

# ARView.DebugOptions.ArrayLiteralElement

The type of the elements of an array literal.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
typealias ArrayLiteralElement = ARView.DebugOptions
```

## See Also

### Creating a debug option set

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

typealias Element

The element type of the option set.

init(rawValue: Int)

Create a debug options enumeration from a raw value.

let rawValue: Int

Options for drawing overlay content in a scene that aids in debugging the scene.

