

- SwiftUI
-  MenuOrder 

Structure

# MenuOrder

The order in which a menu presents its content.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct MenuOrder
```

## Overview

You can configure the preferred menu order using the menuOrder(_:) view modifier.

## Topics

### Getting menu orders

static let automatic: MenuOrder

The ordering of the menu chosen by the system for the current context.

static let fixed: MenuOrder

Order items from top to bottom.

static let priority: MenuOrder

Keep the first items closest to user’s interaction point.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Setting a preferred order

func menuOrder(MenuOrder) -> some View

Sets the preferred order of items for menus presented from this view.

var menuOrder: MenuOrder

The preferred order of items for menus presented from this view.

