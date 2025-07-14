

- SwiftUI
- ObservedObject
-  init(initialValue:) 

Initializer

# init(initialValue:)

Creates an observed object with an initial value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
init(initialValue: ObjectType)
```

## Parameters 

`initialValue`  

An initial value.

## Discussion

This initializer has the same behavior as the init(wrappedValue:) initializer. See that initializer for more information.

## See Also

### Creating an observed object

init(wrappedValue: ObjectType)

Creates an observed object with an initial wrapped value.

