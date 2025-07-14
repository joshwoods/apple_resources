

- SwiftUI
- View
-  focusedValue(\_:\_:) 

Instance Method

# focusedValue(\_:\_:)

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func focusedValue(
    _ keyPath: WritableKeyPath,
    _ value: Value
) -> some View
```

Show all declarations

## Parameters 

`keyPath`  

The key path to associate `value` with when adding it to the existing table of exported focus values.

`value`  

The focus value to export.

## Return Value

A modified representation of this view.

## See Also

### Exposing value types to focused views

func focusedValue&lt;T>(T?) -> some View

Sets the focused value for the given object type.

func focusedSceneValue&lt;T>(T?) -> some View

Sets the focused value for the given object type at a scene-wide scope.

func focusedSceneValue(_:_:)

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused scene.

struct FocusedValues

A collection of state exported by the focused view and its ancestors.

