

- SwiftUI
- WKApplicationDelegateAdaptor
-  init(\_:) 

Initializer

# init(\_:)

Creates an `WKApplicationDelegateAdaptor` using a WatchKit Application Delegate.

watchOS 10.0+

``` source
@MainActor @preconcurrency
init(_ delegateType: DelegateType.Type = DelegateType.self)
```

Available when `DelegateType` inherits `NSObject`, `DelegateType` conforms to `Observable`, and `DelegateType` conforms to `WKApplicationDelegate`.

Show all declarations

## Discussion

The framework will initialize the provided delegate and manage its lifetime, calling out to it when appropriate after performing its own work.

Note

The instantiated delegate will be placed in the Environment and may be accessed by using the `@Environment` property wrapper in the view hierarchy.

