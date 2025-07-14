

- SwiftUI
- State
-  init(wrappedValue:) 

Initializer

# init(wrappedValue:)

Creates a state property that stores an initial wrapped value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(wrappedValue value: Value)
```

## Parameters 

`value`  

An initial value to store in the state property.

## Discussion

You don’t call this initializer directly. Instead, SwiftUI calls it for you when you declare a property with the `@State` attribute and provide an initial value:

```
struct MyView: View {
    @State private var isPlaying: Bool = false

    // ...
}
```

SwiftUI initializes the state’s storage only once for each container instance that you declare. In the above code, SwiftUI creates `isPlaying` only the first time it initializes a particular instance of `MyView`. On the other hand, each instance of `MyView` creates a distinct instance of the state. For example, each of the views in the following VStack has its own `isPlaying` value:

```
var body: some View {
    VStack {
        MyView()
        MyView()
    }
}
```

## See Also

### Creating a state

init(initialValue: Value)

Creates a state property that stores an initial value.

init()

Creates a state property without an initial value.

