

- Assignables
- AssignableDocumentView
-  defersSystemGestures(on:) 

Instance Method

# defersSystemGestures(on:)

Sets the screen edge from which you want your gesture to take precedence over the system gesture.

AssignablesSwiftUIiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
nonisolated
func defersSystemGestures(on edges: Edge.Set) -> some View
```

## Parameters 

`edges`  

A value that indicates the screen edge from which you want your gesture to take precedence over the system gesture.

## Discussion

The following code defers the vertical screen edges system gestures of a given canvas.

```
struct DeferredView: View {
    var body: some View {
        Canvas()
            .defersSystemGestures(on: .vertical)
    }
}
```

