

- SwiftUI
- EnvironmentValues
-  init() 

Initializer

# init()

Creates an environment values instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init()
```

## Discussion

You don’t typically create an instance of EnvironmentValues directly. Doing so would provide access only to default values that don’t update based on system settings or device characteristics. Instead, you rely on an environment values’ instance that SwiftUI manages for you when you use the Environment property wrapper and the environment(_:_:) view modifier.

## See Also

### Creating and accessing values

subscript(_:)

Accesses the environment value associated with a custom key.

var description: String

A string that represents the contents of the environment values instance.

