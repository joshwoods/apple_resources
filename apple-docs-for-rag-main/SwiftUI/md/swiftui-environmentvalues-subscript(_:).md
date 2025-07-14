

- SwiftUI
- EnvironmentValues
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the environment value associated with a custom key.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
subscript(key: K.Type) -> K.Value where K : EnvironmentKey { get set }
```

Show all declarations

## Overview

Create a custom environment value by declaring a new property in an extension to the environment values structure and applying the Entry() macro to the variable declaration:

```
extension EnvironmentValues {
    @Entry var myCustomValue: String = "Default value"
}
```

You use custom environment values the same way you use system-provided values, setting a value with the environment(_:_:) view modifier, and reading values with the Environment property wrapper. You can also provide a dedicated view modifier as a convenience for setting the value:

```
extension View {
    func myCustomValue(_ myCustomValue: String) -> some View {
        environment(\.myCustomValue, myCustomValue)
    }
}
```

## See Also

### Creating and accessing values

init()

Creates an environment values instance.

var description: String

A string that represents the contents of the environment values instance.

