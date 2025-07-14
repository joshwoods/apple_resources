

- SwiftUI
- EnvironmentValues
-  isPresented 

Instance Property

# isPresented

A Boolean value that indicates whether the view associated with this environment is currently presented.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var isPresented: Bool { get }
```

## Discussion

You can read this value like any of the other EnvironmentValues by creating a property with the Environment property wrapper:

```
@Environment(\.isPresented) private var isPresented
```

Read the value inside a view if you need to know when SwiftUI presents that view. For example, you can take an action when SwiftUI presents a view by using the onChange(of:initial:_:) modifier:

```
.onChange(of: isPresented) { _, isPresented in
    if isPresented {
        // Do something when first presented.
    }
}
```

This behaves differently than onAppear(perform:), which SwiftUI can call more than once for a given presentation, like when you navigate back to a view that’s already in the navigation hierarchy.

To dismiss the currently presented view, use dismiss.

## See Also

### Dismissing a presentation

var dismiss: DismissAction

An action that dismisses the current presentation.

struct DismissAction

An action that dismisses a presentation.

func interactiveDismissDisabled(Bool) -> some View

Conditionally prevents interactive dismissal of presentations like popovers, sheets, and inspectors.

