

- SwiftUI
- StateObject
-  wrappedValue 

Instance Property

# wrappedValue

The underlying value referenced by the state object.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
var wrappedValue: ObjectType { get }
```

## Discussion

The wrapped value property provides primary access to the value’s data. However, you don’t typically access it directly. Instead, SwiftUI accesses this property for you when you refer to the variable that you create with the `@StateObject` attribute:

```
@StateObject private var contact = Contact()

var body: some View {
    Text(contact.name) // Reads name from contact's wrapped value.
}
```

When you change a wrapped value, you can access the new value immediately. However, SwiftUI updates views that display the value asynchronously, so the interface might not update immediately.

## See Also

### Getting the value

var projectedValue: ObservedObject&lt;ObjectType>.Wrapper

A projection of the state object that creates bindings to its properties.

