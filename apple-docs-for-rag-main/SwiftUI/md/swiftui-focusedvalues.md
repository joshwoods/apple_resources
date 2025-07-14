

- SwiftUI
-  FocusedValues 

Structure

# FocusedValues

A collection of state exported by the focused view and its ancestors.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct FocusedValues
```

## Topics

### Getting the value for a key

subscript&lt;Key>(Key.Type) -> Key.Value?

Reads and writes values associated with a given focused value key.

## Relationships

### Conforms To

- Copyable
- Equatable

## See Also

### Exposing value types to focused views

func focusedValue&lt;T>(T?) -> some View

Sets the focused value for the given object type.

func focusedValue(_:_:)

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused view hierarchy.

func focusedSceneValue&lt;T>(T?) -> some View

Sets the focused value for the given object type at a scene-wide scope.

func focusedSceneValue(_:_:)

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused scene.

