

- SwiftUI
- Bindable
-  subscript(dynamicMember:) 

Instance Subscript

# subscript(dynamicMember:)

Returns a binding to the value of a given key path.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
subscript(dynamicMember keyPath: ReferenceWritableKeyPath) -> Binding { get }
```

## See Also

### Getting the value

var wrappedValue: Value

The wrapped object.

var projectedValue: Bindable&lt;Value>

The bindable wrapper for the object that creates bindings to its properties using dynamic member lookup.

