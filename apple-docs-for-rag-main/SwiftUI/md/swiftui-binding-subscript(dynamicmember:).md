

- SwiftUI
- Binding
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Returns a binding to the resulting value of a given key path.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
subscript(dynamicMember keyPath: WritableKeyPath) -> Binding { get }
```

## Parameters 

`keyPath`  

A key path to a specific resulting value.

## Return Value

A new binding.

## See Also

### Getting the value

var wrappedValue: Value

The underlying value referenced by the binding variable.

var projectedValue: Binding&lt;Value>

A projection of the binding value that returns a binding.

