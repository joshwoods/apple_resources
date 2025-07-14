

- RealityKit
- ARView
- ARView.DebugOptions
-  ARView.DebugOptions.Element 

Type Alias

# ARView.DebugOptions.Element

The element type of the option set.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+

``` source
typealias Element = ARView.DebugOptions
```

## Discussion

To inherit all the default implementations from the `OptionSet` protocol, the `Element` type must be `Self`, the default.

## See Also

### Creating a debug option set

init()

Creates an empty option set.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init(arrayLiteral: Self.Element...)

Creates a set containing the elements of the given array literal.

typealias ArrayLiteralElement

The type of the elements of an array literal.

init(rawValue: Int)

Create a debug options enumeration from a raw value.

let rawValue: Int

Options for drawing overlay content in a scene that aids in debugging the scene.

