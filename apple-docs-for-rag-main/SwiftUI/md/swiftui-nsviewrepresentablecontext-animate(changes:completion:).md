

- SwiftUI
- NSViewRepresentableContext
-  animate(changes:completion:) 

Instance Method

# animate(changes:completion:)

Animates changes using the animation in the current transaction.

macOS 15.0+

``` source
@backDeployed(before: macOS 15.4)
@MainActor @preconcurrency
func animate(
    changes: () -> Void,
    completion: (() -> Void)? = nil
)
```

Available when `View` conforms to `NSViewRepresentable`.

## Parameters 

`changes`  

A closure that changes animatable properties.

`completion`  

A closure to execute after the animation completes.

## Discussion

This combines animate(with:changes:completion:) with the current transaction’s animation. When you start a SwiftUI animation using withAnimation(_:_:) and have a mutated SwiftUI state that causes the representable object to update, use this method to animate changes in the representable object using the same `Animation` timing.

```
struct ContentView: View {
    @State private var isCollapsed = false
    var body: some View {
        ZStack {
            MyDetailView(isCollapsed: isCollapsed)
            MyRepresentable(isCollapsed: $isCollapsed)
            Button("Collapse Content") {
                withAnimation(.bouncy) {
                    isCollapsed = true
                }
            }
        }
    }
}

struct MyRepresentable: NSViewRepresentable {
    @Binding var isCollapsed: Bool

    func updateNSView(_ nsView: NSViewType, context: Context) {
        if isCollapsed && !nsView.isCollapsed {
            context.animate {
                nsView.collapseSubview()
                nsView.layoutSubtreeIfNeeded()
            }
        }
    }
}
```

