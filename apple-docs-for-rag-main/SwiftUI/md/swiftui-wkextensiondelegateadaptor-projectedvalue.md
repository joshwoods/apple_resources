

- SwiftUI
- WKExtensionDelegateAdaptor
-  projectedValue 

Instance Property

# projectedValue

A projection of the observed object that provides bindings to its properties.

watchOS 7.0+

``` source
@MainActor @preconcurrency
var projectedValue: ObservedObject.Wrapper { get }
```

Available when `DelegateType` inherits `NSObject`, `DelegateType` conforms to `ObservableObject`, and `DelegateType` conforms to `WKExtensionDelegate`.

## Discussion

Use the projected value to get a binding to a value that the delegate publishes. Access the projected value by prefixing the name of the delegate instance with a dollar sign (`$`). For example, you might publish a Boolean value in your extension delegate:

```
class MyExtensionDelegate: NSObject, WKExtensionDelegate, ObservableObject {
    @Published var isEnabled = false

    // ...
}
```

If you declare the delegate in your App using the WKExtensionDelegateAdaptor property wrapper, you can get the delegate that SwiftUI instantiates from the environment and access a binding to its published values from any view in your extension:

```
struct MyView: View {
    @EnvironmentObject private var extensionDelegate: MyExtensionDelegate

    var body: some View {
        Toggle("Enabled", isOn: $extensionDelegate.isEnabled)
    }
}
```

## See Also

### Getting the delegate adaptor

var wrappedValue: DelegateType

The underlying delegate.

