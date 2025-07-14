

- AppKit
- NSApplication
-  servicesMenu 

Instance Property

# servicesMenu

The app’s Services menu.

macOS

``` source
@MainActor
var servicesMenu: NSMenu? { get set }
```

## Discussion

This property contains the app’s Services menu or `nil` if that menu has not been created. You can assign a new value to the property to set the Services menu for your app.

## See Also

### Managing the Services Menu

func registerServicesMenuSendTypes([NSPasteboard.PasteboardType], returnTypes: [NSPasteboard.PasteboardType])

Registers the pasteboard types the receiver can send and receive in response to service requests.

