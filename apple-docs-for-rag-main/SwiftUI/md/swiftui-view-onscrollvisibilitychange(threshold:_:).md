

- SwiftUI
- View
-  onScrollVisibilityChange(threshold:\_:) 

Instance Method

# onScrollVisibilityChange(threshold:\_:)

Adds an action to be called when the view crosses the threshold to be considered on/off screen.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
nonisolated
func onScrollVisibilityChange(
    threshold: Double = 0.5,
    _ action: @escaping (Bool) -> Void
) -> some View
```

## Parameters 

`threshold`  

The amount required to be visible within the viewport of the the parent view before the `action` is fired. By default when the view has crossed more than 50% on-screen, the action will be called.

`action`  

The action which will be called when the threshold has been reached.

## Discussion

Use this modifier to be informed when the view has crossed the provided threshold to be considered on/off screen.

```
struct VideoPlayer: View {
    @State var playing: Bool

    var body: some View {
        Group {
            // ...
        }
        .onScrollVisibilityChange(threshold: 0.2) { isVisible in
            playing = isVisible
        }
    }
}
```

When the view appears on-screen, the action will be called if the threshold has already been reached.

## See Also

### Responding to scroll view changes

func onScrollGeometryChange&lt;T>(for: T.Type, of: (ScrollGeometry) -> T, action: (T, T) -> Void) -> some View

Adds an action to be performed when a value, created from a scroll geometry, changes.

func onScrollTargetVisibilityChange&lt;ID>(idType: ID.Type, threshold: Double, ([ID]) -> Void) -> some View

Adds an action to be called with information about what views would be considered visible.

func onScrollPhaseChange(_:)

Adds an action to perform when the scroll phase of the first scroll view in the hierarchy changes.

struct ScrollGeometry

A type that defines the geometry of a scroll view.

enum ScrollPhase

A type that describes the state of a scroll gesture of a scrollable view like a scroll view.

struct ScrollPhaseChangeContext

A type that provides you with more content when the phase of a scroll view changes.

