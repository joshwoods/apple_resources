

- macOS Release Notes
-  AppKit Release Notes for macOS Ventura 13 

Article

# AppKit Release Notes for macOS Ventura 13

Update your apps to use new features, and test your apps against API changes.

## Overview

AppKit in macOS Ventura 13 includes new features, as well as API changes and deprecations.

### New Features

#### NSColorWell

- Color wells have a modernized appearance and two new styles in macOS 13. See the new colorWellStyle property and associated NSColorWell.Style type for more information on configuring a color well’s style.

- The two new color well styles, NSColorWell.Style.minimal and NSColorWell.Style.expanded, offer a pull-down capability. By default, interacting with the well displays a popover with a palette of color choices for quick picking. Applications can customize this interaction using the new pulldownTarget and pulldownAction properties.

- Borderless color wells will be deprecated in a future release. The isBordered property has been annotated as such.

#### NSComboButton

- macOS 13 introduces a new type of control: NSComboButton. NSComboButton provides the functionality of a pull-down menu along with a primary action.

- NSComboButton is configurable with two styles, NSComboButton.Style.split and NSComboButton.Style.unified. Refer to the class documentation for guidance on the appearance and behavior of each case.

#### NSNib

- The doc://com.apple.documentation/documentation/appkit/nsnib/1547299-initwithcontentsofurl initializer (deprecated since 10.8) now throws an assertion. Use init(nibNamed:bundle:) instead.

#### NSTableView and NSOutlineView

- On macOS 13 and higher, changing the autosaveName property from one value to another will automatically persist autosave data for the old value before changing to the new value. Setting `autosaveName` to `nil` removes the persistence data for the previously set `autosaveName`.

- NSTableView and NSOutlineView now automatically estimate row heights for view-based table views whose delegates implement tableView(_:heightOfRow:) and provide variable row heights. This provides performance improvements for table views with large numbers of rows by reducing the frequency of the calls to tableView(_:heightOfRow:).

Note

To get the benefit of row height estimation, the table view must be view-based and not override rect(ofRow:), row(at:), or rows(in:).

- For cell-based table views, checking Autosave Column Information in Interface Builder now correctly persists column information for columns that have automatic column identifiers.

- For apps linked against the macOS 13 SDK, NSTableRowView and subclasses that override drawSeparator(in:) now draw their separators correctly, even when displayed as floating group rows.

### Deprecations

#### NSToolbar

- Placing an NSToolbarItem item taller than the toolbar height is not supported and will result in clipping. When drawing a custom badge, use alignmentRectInsets of the control to describe where the button is and draw within the inset area.

