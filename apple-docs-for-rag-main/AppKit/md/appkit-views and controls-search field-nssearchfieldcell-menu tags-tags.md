

- AppKit
- Views and Controls
- Search Field
- NSSearchFieldCell
-  Menu tags 

API Collection

# Menu tags

Constants for identifying special menu items in the search-menu template.

## Overview

When an `NSSearchFieldCell` object dynamically constructs the actual search menu from this template, it shows or hides the tagged items as directed.

## Topics

### Constants

class let recentsTitleMenuItemTag: Int

The menu item that provides the title of the menu group for recent search strings.

class let recentsMenuItemTag: Int

The location of recent search strings in the “recents” menu group.

class let clearRecentsMenuItemTag: Int

The menu item for clearing the current set of recent string searches in the menu.

class let noRecentsMenuItemTag: Int

The menu item that describes a lack of recent search strings.

