

- SwiftUI
- Bindable
-  projectedValue 

Instance Property

# projectedValue

The bindable wrapper for the object that creates bindings to its properties using dynamic member lookup.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var projectedValue: Bindable { get }
```

## See Also

### Getting the value

var wrappedValue: Value

The wrapped object.

subscript&lt;Subject>(dynamicMember _: ReferenceWritableKeyPath&lt;Value, Subject>) -> Binding&lt;Subject>

Returns a binding to the value of a given key path.

