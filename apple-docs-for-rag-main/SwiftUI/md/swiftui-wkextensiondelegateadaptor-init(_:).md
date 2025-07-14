

- SwiftUI
- WKExtensionDelegateAdaptor
-  init(\_:) 

Initializer

# init(\_:)

Creates a WatchKit extension delegate adaptor using an observable delegate.

watchOS 10.0+

``` source
@MainActor @preconcurrency
init(_ delegateType: DelegateType.Type = DelegateType.self)
```

Available when `DelegateType` inherits `NSObject`, `DelegateType` conforms to `Observable`, and `DelegateType` conforms to `WKExtensionDelegate`.

Show all declarations

## Parameters 

`delegateType`  

The type of extension delegate that you define in your app, which conforms to the WKExtensionDelegate and Observable protocols.

## Discussion

Call this initializer indirectly by creating a property with the WKExtensionDelegateAdaptor property wrapper from inside your App declaration:

```
@main
struct MyApp: App {
    @WKExtensionDelegateAdaptor private var extensionDelegate: MyExtensionDelegate

    var body: some Scene { ... }
}
```

SwiftUI initializes the delegate and manages its lifetime, calling it as needed to handle extension delegate callbacks.

SwiftUI invokes this method when your app delegate conforms to the Observable protocol. In this case, SwiftUI automatically places the delegate in the Environment. You can access such a delegate from any scene or view in your app using the Environment property wrapper:

```
@Environment(MyAppDelegate.self) private var appDelegate
```

If your delegate isn’t observable, SwiftUI invokes the init(_:) initializer rather than this one, and doesn’t put the delegate instance in the environment.

