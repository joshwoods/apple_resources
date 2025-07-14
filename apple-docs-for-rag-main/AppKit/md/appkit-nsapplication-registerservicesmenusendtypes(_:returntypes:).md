

- AppKit
- NSApplication
-  registerServicesMenuSendTypes(\_:returnTypes:) 

Instance Method

# registerServicesMenuSendTypes(\_:returnTypes:)

Registers the pasteboard types the receiver can send and receive in response to service requests.

macOS

``` source
@MainActor
func registerServicesMenuSendTypes(
    _ sendTypes: [NSPasteboard.PasteboardType],
    returnTypes: [NSPasteboard.PasteboardType]
)
```

## Parameters 

`sendTypes`  

An array of `NSString` objects, each of which corresponds to a particular pasteboard type that the app can send.

`returnTypes`  

An array of `NSString` objects, each of which corresponds to a particular pasteboard type that the app can receive.

## Discussion

If the receiver has a Services menu, a menu item is added for each service provider that can accept one of the specified `sendTypes` or return one of the specified `returnTypes`. You should typically invoke this method at app startup time or when an object that can use services is created. You can invoke it more than once—its purpose is to ensure there is a menu item for every service the app can use. The event-handling mechanism will dynamically enable the individual items to indicate which services are currently appropriate. All the `NSResponder` objects in your app (typically `NSView` objects) should register every possible type they can send and receive by sending this message to `NSApp`.

## See Also

### Related Documentation

func validRequestor(forSendType: NSPasteboard.PasteboardType?, returnType: NSPasteboard.PasteboardType?) -> Any?

Indicates whether the receiver can send and receive the specified pasteboard types.

### Managing the Services Menu

var servicesMenu: NSMenu?

The app’s Services menu.

