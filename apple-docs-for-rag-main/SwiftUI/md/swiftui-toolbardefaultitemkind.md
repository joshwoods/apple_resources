

- SwiftUI
-  ToolbarDefaultItemKind 

Structure

# ToolbarDefaultItemKind

A kind of toolbar item a `View` adds by default.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
struct ToolbarDefaultItemKind
```

## Overview

`View`s can add toolbar items clients may wish to remove or customize. A default item kind can be passed to the toolbar(removing:) modifier to remove the item. Documentation on the `View` placing the default item should reference the `ToolbarDefaultItemKind` used to remove the item.

## Topics

### Getting the default item types

static let sidebarToggle: ToolbarDefaultItemKind

The sidebar toggle toolbar item a `NavigationSplitView` adds by default.

### Type Properties

static let title: ToolbarDefaultItemKind

The title and subtitle shown in title bar / navigation bar.

## See Also

### Removing default items

func toolbar(removing: ToolbarDefaultItemKind?) -> some View

Remove a toolbar item present by default

