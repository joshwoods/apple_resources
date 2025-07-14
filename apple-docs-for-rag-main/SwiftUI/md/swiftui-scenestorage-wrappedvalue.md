

- SwiftUI
- SceneStorage
-  wrappedValue 

Instance Property

# wrappedValue

The underlying value referenced by the state variable.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var wrappedValue: Value { get nonmutating set }
```

## Discussion

This works identically to `State.wrappedValue`.

See Also

State.wrappedValue

## See Also

### Getting the value

var projectedValue: Binding&lt;Value>

A binding to the state value.

