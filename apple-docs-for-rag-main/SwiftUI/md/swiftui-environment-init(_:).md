

- SwiftUI
- Environment
-  init(\_:) 

Initializer

# init(\_:)

Creates an environment property to read the specified key path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(_ keyPath: KeyPath)
```

Show all declarations

## Parameters 

`keyPath`  

A key path to a specific resulting value.

## Discussion

Don’t call this initializer directly. Instead, declare a property with the Environment property wrapper, and provide the key path of the environment value that the property should reflect:

```
struct MyView: View {
    @Environment(\.colorScheme) var colorScheme: ColorScheme

    // ...
}
```

SwiftUI automatically updates any parts of `MyView` that depend on the property when the associated environment value changes. You can’t modify the environment value using a property like this. Instead, use the environment(_:_:) view modifier on a view to set a value for a view hierarchy.

