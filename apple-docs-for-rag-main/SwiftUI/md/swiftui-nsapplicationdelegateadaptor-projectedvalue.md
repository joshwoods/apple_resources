

- SwiftUI
- NSApplicationDelegateAdaptor
-  projectedValue 

Instance Property

# projectedValue

A projection of the observed object that provides bindings to its properties.

macOS 11.0+

``` source
@MainActor @preconcurrency
var projectedValue: ObservedObject.Wrapper { get }
```

Available when `DelegateType` inherits `NSObject`, `DelegateType` conforms to `NSApplicationDelegate`, and `DelegateType` conforms to `ObservableObject`.

## Discussion

Use the projected value to get a binding to a value that the delegate publishes. Access the projected value by prefixing the name of the delegate instance with a dollar sign (`$`). For example, you might publish a Boolean value in your application delegate:

```
class MyAppDelegate: NSObject, NSApplicationDelegate, ObservableObject {
    @Published var isEnabled = false

    // ...
}
```

If you declare the delegate in your App using the NSApplicationDelegateAdaptor property wrapper, you can get the delegate that SwiftUI instantiates from the environment and access a binding to its published values from any view in your app:

```
struct MyView: View {
    @EnvironmentObject private var appDelegate: MyAppDelegate

    var body: some View {
        Toggle("Enabled", isOn: $appDelegate.isEnabled)
    }
}
```

## See Also

### Getting the delegate adaptor

var wrappedValue: DelegateType

The underlying delegate.

