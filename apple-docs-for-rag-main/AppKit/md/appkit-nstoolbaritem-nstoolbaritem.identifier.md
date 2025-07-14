

- AppKit
- NSToolbarItem
-  NSToolbarItem.Identifier 

Structure

# NSToolbarItem.Identifier

Constants for the standard toolbar items that the system provides.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
struct Identifier
```

## Overview

If you configure an NSToolbarItem in Interface Builder with one of the standard identifiers, AppKit configures the toolbar item for you automatically when you load your interface. Similarly, if your toolbar delegate returns them as part of the default or allowed set of items, AppKit handles their configuration. When your delegate provides standard identifiers, AppKit doesn’t call the toolbar(_:itemForItemIdentifier:willBeInsertedIntoToolbar:) method for them.

## Topics

### Getting the standard item identifiers

static let space: NSToolbarItem.Identifier

The identifier for a toolbar item that displays an empty space with a standard fixed size.

static let flexibleSpace: NSToolbarItem.Identifier

The identifier for a toolbar item that displays an empty space with a flexible width.

static let cloudSharing: NSToolbarItem.Identifier

The identifier for a toolbar item that tells your app to display the iCloud sharing interface.

static let print: NSToolbarItem.Identifier

The identifier for a toolbar item that tells your app to print the current document.

static let showColors: NSToolbarItem.Identifier

The identifier for a toolbar item that shows the standard color panel.

static let showFonts: NSToolbarItem.Identifier

The identifier for a toolbar item that shows the standard font panel.

static let toggleSidebar: NSToolbarItem.Identifier

The identifier for a toolbar item that displays a sidebar.

static let sidebarTrackingSeparator: NSToolbarItem.Identifier

The identifier for a toolbar item that displays a tracking separator aligned with the sidebar divider in a split view.

static let primarySidebarTrackingSeparatorItemIdentifier: NSToolbarItem.Identifier

The identifier for a toolbar item that displays a tracking separator aligned with the primary divider in a split view.

static let supplementarySidebarTrackingSeparatorItemIdentifier: NSToolbarItem.Identifier

The identifier for a toolbar item that displays a tracking separator aligned with the secondary divider in a split view.

static let inspectorTrackingSeparator: NSToolbarItem.Identifier

static let toggleInspector: NSToolbarItem.Identifier

### Creating an identifier

init(String)

Creates a toolbar item identifier.

init(rawValue: String)

Creates a toolbar item identifier with the specified raw value.

### Deprecated

static let customizeToolbar: NSToolbarItem.Identifier

The Customize item, which shows the customization palette.

Deprecated

static let separator: NSToolbarItem.Identifier

The Separator item.

Deprecated

### Type Properties

static let writingToolsItemIdentifier: NSToolbarItem.Identifier

A standard item that is configured to send -showWritingTools: to the firstResponder when invoked.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the toolbar item’s identity

var itemIdentifier: NSToolbarItem.Identifier

The value you use to identify the toolbar item.

