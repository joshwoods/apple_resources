

- SwiftUI
- NSApplicationDelegateAdaptor
-  init(\_:) 

Initializer

# init(\_:)

Creates an AppKit app delegate adaptor using an observable delegate.

macOS 14.0+

``` source
@MainActor @preconcurrency
init(_ delegateType: DelegateType.Type = DelegateType.self)
```

Available when `DelegateType` inherits `NSObject`, `DelegateType` conforms to `NSApplicationDelegate`, and `DelegateType` conforms to `Observable`.

Show all declarations

## Parameters 

`delegateType`  

The type of application delegate that you define in your app, which conforms to the NSApplicationDelegate and Observable protocols.

## Discussion

Call this initializer indirectly by creating a property with the NSApplicationDelegateAdaptor property wrapper from inside your App declaration:

```
@main
struct MyApp: App {
    @NSApplicationDelegateAdaptor private var appDelegate: MyAppDelegate

    var body: some Scene { ... }
}
```

SwiftUI initializes the delegate and manages its lifetime, calling it as needed to handle application delegate callbacks.

SwiftUI invokes this method when your app delegate conforms to the Observable protocol. In this case, SwiftUI automatically places the delegate in the Environment. You can access such a delegate from any scene or view in your app using the Environment property wrapper:

```
@Environment(MyAppDelegate.self) private var appDelegate
```

If your delegate isn’t observable, SwiftUI invokes the init(_:) initializer rather than this one, and doesn’t put the delegate instance in the environment.

