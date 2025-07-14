

- SwiftUI
-  WKApplicationDelegateAdaptor 

Structure

# WKApplicationDelegateAdaptor

A property wrapper that is used in `App` to provide a delegate from WatchKit.

watchOS 7.0+

``` source
@MainActor @preconcurrency @propertyWrapper
struct WKApplicationDelegateAdaptor where DelegateType : NSObject, DelegateType : WKApplicationDelegate
```

## Mentioned in 

Migrating to the SwiftUI life cycle

## Topics

### Creating a delegate adaptor

init(_:)

Creates an `WKApplicationDelegateAdaptor` using a WatchKit Application Delegate.

### Getting the delegate adaptor

var projectedValue: ObservedObject&lt;DelegateType>.Wrapper

A projection of the observed object that creates bindings to its properties using dynamic member lookup.

var wrappedValue: DelegateType

The underlying delegate.

## Relationships

### Conforms To

- DynamicProperty
- Sendable

## See Also

### Targeting watchOS

struct WKExtensionDelegateAdaptor

A property wrapper type that you use to create a WatchKit extension delegate.

