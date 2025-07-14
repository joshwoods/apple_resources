

- SwiftUI
- Bindable
-  wrappedValue 

Instance Property

# wrappedValue

The wrapped object.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
var wrappedValue: Value
```

## See Also

### Getting the value

var projectedValue: Bindable&lt;Value>

The bindable wrapper for the object that creates bindings to its properties using dynamic member lookup.

subscript&lt;Subject>(dynamicMember _: ReferenceWritableKeyPath&lt;Value, Subject>) -> Binding&lt;Subject>

Returns a binding to the value of a given key path.

