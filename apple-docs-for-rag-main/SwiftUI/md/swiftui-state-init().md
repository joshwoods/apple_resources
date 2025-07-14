

- SwiftUI
- State
-  init() 

Initializer

# init()

Creates a state property without an initial value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init()
```

Available when `Value` conforms to `ExpressibleByNilLiteral`.

## Discussion

This initializer behaves like the init(wrappedValue:) initializer with an input of `nil`. See that initializer for more information.

## See Also

### Creating a state

init(wrappedValue: Value)

Creates a state property that stores an initial wrapped value.

init(initialValue: Value)

Creates a state property that stores an initial value.

