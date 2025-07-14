

- SwiftUI
- View
-  focusedSceneValue(\_:) 

Instance Method

# focusedSceneValue(\_:)

Sets the focused value for the given object type at a scene-wide scope.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func focusedSceneValue(_ object: T?) -> some View where T : AnyObject, T : Observable
```

## Discussion

Important

This initializer only accepts objects conforming to the `Observable` protocol. For reading environment objects that conform to `ObservableObject`, use `focusedObject(_:)`, instead.

To read this value, use the `FocusedValue` property wrapper.

## See Also

### Exposing value types to focused views

func focusedValue&lt;T>(T?) -> some View

Sets the focused value for the given object type.

func focusedValue(_:_:)

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused view hierarchy.

func focusedSceneValue(_:_:)

Modifies this view by injecting a value that you provide for use by other views whose state depends on the focused scene.

struct FocusedValues

A collection of state exported by the focused view and its ancestors.

