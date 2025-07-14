

- SwiftUI
- WKApplicationDelegateAdaptor
-  wrappedValue 

Instance Property

# wrappedValue

The underlying delegate.

watchOS 7.0+

``` source
@MainActor @preconcurrency
var wrappedValue: DelegateType { get }
```

## See Also

### Getting the delegate adaptor

var projectedValue: ObservedObject&lt;DelegateType>.Wrapper

A projection of the observed object that creates bindings to its properties using dynamic member lookup.

