

- AppKit
- NSAlert
-  icon 

Instance Property

# icon

The custom icon displayed in the alert.

macOS

``` source
@MainActor
var icon: NSImage! { get set }
```

## Discussion

By default, the image used in an alert is the app icon. If you set this property’s value, your specified custom image is used in place of the app icon.

If you’ve set a custom alert icon, you can clear it by setting this property’s value to `nil`, which restores use of the app icon for the alert.

