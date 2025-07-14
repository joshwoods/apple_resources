

- SwiftUI
- Binding
-  wrappedValue 

Instance Property

# wrappedValue

The underlying value referenced by the binding variable.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
var wrappedValue: Value { get nonmutating set }
```

## Discussion

This property provides primary access to the value’s data. However, you don’t access `wrappedValue` directly. Instead, you use the property variable created with the Binding attribute. In the following code example, the binding variable `isPlaying` returns the value of `wrappedValue`:

```
struct PlayButton: View {
    @Binding var isPlaying: Bool

    var body: some View {
        Button(isPlaying ? "Pause" : "Play") {
            isPlaying.toggle()
        }
    }
}
```

When a mutable binding value changes, the new value is immediately available. However, updates to a view displaying the value happens asynchronously, so the view may not show the change immediately.

## See Also

### Getting the value

var projectedValue: Binding&lt;Value>

A projection of the binding value that returns a binding.

subscript&lt;Subject>(dynamicMember _: WritableKeyPath&lt;Value, Subject>) -> Binding&lt;Subject>

Returns a binding to the resulting value of a given key path.

