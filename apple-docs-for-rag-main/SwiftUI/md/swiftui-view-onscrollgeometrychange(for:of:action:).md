

- SwiftUI
- View
-  onScrollGeometryChange(for:of:action:) 

Instance Method

# onScrollGeometryChange(for:of:action:)

Adds an action to be performed when a value, created from a scroll geometry, changes.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func onScrollGeometryChange(
    for type: T.Type,
    of transform: @escaping (ScrollGeometry) -> T,
    action: @escaping (T, T) -> Void
) -> some View where T : Equatable
```

## Parameters 

`type`  

The type of value transformed from a ScrollGeometry.

`transform`  

A closure that transforms a ScrollGeometry to your type.

`action`  

A closure to run when the transformed data changes.

## Discussion

The geometry of a scroll view changes frequently while scrolling. You should avoid updating large parts of your app whenever the scroll geometry changes. To aid in this, you provide two closures to this modifier:

- transform: This converts a value of ScrollGeometry to a your own data type.

- action: This provides the data type you created in `of` and is called whenever the data type changes.

For example, you can use this modifier to know when the user scrolls a scroll view beyond the top of its content. In the following example, the data type you convert to is a `Bool` and the action is called whenever the `Bool` changes.

```
@Binding var isBeyondZero: Bool

ScrollView {
    // ...
}
.onScrollGeometryChange(for: Bool.self) { geometry in
    geometry.contentOffset.y 

If multiple scroll views are found within the view hierarchy, only the first one will invoke the closure you provide and a runtime issue will be logged. For example, in the following view, only the vertical scroll view will have its geometry changes invoke the provided closure.

```
VStack {
    ScrollView(.vertical) { ... }
    ScrollView(.horizontal) { ... }
}
.onScrollGeometryChange(for: Bool.self) { geometry in
     ...
} action: { oldValue, newValue in
    ...
}
```

For responding to non-scroll geometry changes, see the onGeometryChange(for:of:action:) modifier.

## See Also

### Responding to scroll view changes

func onScrollTargetVisibilityChange&lt;ID>(idType: ID.Type, threshold: Double, ([ID]) -> Void) -> some View

Adds an action to be called with information about what views would be considered visible.

func onScrollVisibilityChange(threshold: Double, (Bool) -> Void) -> some View

Adds an action to be called when the view crosses the threshold to be considered on/off screen.

func onScrollPhaseChange(_:)

Adds an action to perform when the scroll phase of the first scroll view in the hierarchy changes.

struct ScrollGeometry

A type that defines the geometry of a scroll view.

enum ScrollPhase

A type that describes the state of a scroll gesture of a scrollable view like a scroll view.

struct ScrollPhaseChangeContext

A type that provides you with more content when the phase of a scroll view changes.

