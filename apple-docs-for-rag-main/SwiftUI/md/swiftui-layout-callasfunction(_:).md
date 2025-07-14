

- SwiftUI
- Layout
-  callAsFunction(\_:) 

Instance Method

# callAsFunction(\_:)

Combines the specified views into a single composite view using the layout algorithms of the custom layout container.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func callAsFunction(@ViewBuilder _ content: () -> V) -> some View where V : View
```

## Parameters 

`content`  

A ViewBuilder that contains the views to lay out.

## Return Value

A composite view that combines all the input views.

## Discussion

Don’t call this method directly. SwiftUI calls it when you instantiate a custom layout that conforms to the Layout protocol:

```
BasicVStack { // Implicitly calls callAsFunction.
    Text("A View")
    Text("Another View")
}
```

For information about how Swift uses the `callAsFunction()` method to simplify call site syntax, see Methods with Special Names in *The Swift Programming Language*.

