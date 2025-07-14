

- AppKit
- NSApplication
-  servicesProvider 

Instance Property

# servicesProvider

The object that provides the services the current app advertises in the Services menu of other apps.

macOS

``` source
@MainActor
var servicesProvider: Any? { get set }
```

## Return Value

The app’s service provider object.

## Discussion

The service provider performs all advertised services for the app. When another app requests a service from the current app, the app object forwards the request to its service provider. Service requests can arrive immediately after the service provider is set, so assign an object to this property only when your app is ready to receive requests.

## See Also

### Providing Services

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Indicates whether the receiver can send and receive the specified pasteboard types.

