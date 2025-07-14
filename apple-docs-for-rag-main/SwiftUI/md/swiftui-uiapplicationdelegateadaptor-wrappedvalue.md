

- SwiftUI
- UIApplicationDelegateAdaptor
-  wrappedValue 

Instance Property

# wrappedValue

The underlying app delegate.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor @preconcurrency
var wrappedValue: DelegateType { get }
```

## See Also

### Getting the delegate adaptor

var projectedValue: ObservedObject&lt;DelegateType>.Wrapper

A projection of the observed object that provides bindings to its properties.

