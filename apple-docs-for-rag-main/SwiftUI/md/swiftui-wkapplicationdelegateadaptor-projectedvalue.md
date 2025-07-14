

- SwiftUI
- WKApplicationDelegateAdaptor
-  projectedValue 

Instance Property

# projectedValue

A projection of the observed object that creates bindings to its properties using dynamic member lookup.

watchOS 7.0+

``` source
@MainActor @preconcurrency
var projectedValue: ObservedObject.Wrapper { get }
```

Available when `DelegateType` inherits `NSObject`, `DelegateType` conforms to `ObservableObject`, and `DelegateType` conforms to `WKApplicationDelegate`.

## Discussion

Use the projected value to pass a binding value down a view hierarchy. To get the `projectedValue`, prefix the property variable with `$`.

## See Also

### Getting the delegate adaptor

var wrappedValue: DelegateType

The underlying delegate.

