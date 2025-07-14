

- SwiftUI
- EnvironmentObject
-  projectedValue 

Instance Property

# projectedValue

A projection of the environment object that creates bindings to its properties using dynamic member lookup.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
var projectedValue: EnvironmentObject.Wrapper { get }
```

## Discussion

Use the projected value to pass an environment object down a view hierarchy.

## See Also

### Getting the value

var wrappedValue: ObjectType

The underlying value referenced by the environment object.

struct Wrapper

A wrapper of the underlying environment object that can create bindings to its properties using dynamic member lookup.

