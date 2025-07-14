

- AppKit
- NSToolbar
-  itemIdentifiers 

Instance Property

# itemIdentifiers

An array of itemIdentifiers that represent the current items in the toolbar. Setting this property will set the current items in the toolbar by diffing against items that already exist. Use this with great caution if `allowsUserCustomization` is enabled as it will override any customizations the user has made. This property is key value observable.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
@MainActor
var itemIdentifiers: [NSToolbarItem.Identifier] { get set }
```

