

- AppKit
- NSToolbar
-  identifier 

Instance Property

# identifier

The value you use to identify the toolbar in your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
@MainActor
var identifier: NSToolbar.Identifier { get }
```

## Discussion

Use this property to distinguish toolbars in your app. Multiple toolbars can share the same identifier, and you might do so for windows that display similar content. When two or more toolbars share an identifier, they synchronize their state and display the same set of items.

If the toolbar autosaves its contents, the system associates the configuration data with this identifier.

## See Also

### Related Documentation

var autosavesConfiguration: Bool

A Boolean value that indicates whether the toolbar autosaves its configuration.

### Getting the toolbar’s identity

typealias Identifier

A string value that you use to differentiate your app’s toolbars.

