

- AppKit
- NSDocumentController
-  allowsAutomaticShareMenu 

Instance Property

# allowsAutomaticShareMenu

A Boolean value that the system uses to insert a Share menu in the File menu.

macOS 10.13+

``` source
@MainActor
var allowsAutomaticShareMenu: Bool { get }
```

## Discussion

If your application has any NSDocument subclasses with autosavesInPlace set to `true`, the system defaults `allowsAutomaticShareMenu` to `true`. To disable the Share menu entirely, or to enable custom placement or construction of the share menu, override this property to return `false` in your app.

The system may not insert a Share menu if `allowsAutomaticShareMenu` is `true` and NSDocumentController detects that the app has a Share menu.

## See Also

### Sharing

func standardShareMenuItem() -> NSMenuItem

Returns a menu item that your app uses for sharing the current document.

