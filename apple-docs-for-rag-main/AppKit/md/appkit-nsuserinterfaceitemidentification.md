

- AppKit
-  NSUserInterfaceItemIdentification 

Protocol

# NSUserInterfaceItemIdentification

A set of methods used to associate a unique identifier with objects in your user interface.

macOS

``` source
protocol NSUserInterfaceItemIdentification
```

## Overview

The protocol is adopted by AppKit interface objects to support window restoration, whereby information about window and other interface-related objects is preserved and used to restore the application’s interface during the next launch cycle.

## Topics

### Accessing the User Interface Identifier

var identifier: NSUserInterfaceItemIdentifier?

A string that identifies the user interface item.

**Required**

struct NSUserInterfaceItemIdentifier

## Relationships

### Inherited By

- NSCollectionViewElement
- NSCollectionViewSectionHeaderView

### Conforming Types

- NSActionCell
- NSBox
- NSBrowser
- NSBrowserCell
- NSButton
- NSButtonCell
- NSCell
- NSClipView
- NSCollectionView
- NSCollectionViewItem
- NSColorPanel
- NSColorWell
- NSComboBox
- NSComboBoxCell
- NSComboButton
- NSControl
- NSDatePicker
- NSDatePickerCell
- NSFontPanel
- NSForm
- NSFormCell
- NSGridView
- NSImageCell
- NSImageView
- NSLayoutGuide
- NSLevelIndicator
- NSLevelIndicatorCell
- NSMatrix
- NSMenu
- NSMenuItem
- NSMenuItemCell
- NSOpenGLView
- NSOpenPanel
- NSOutlineView
- NSPageController
- NSPanel
- NSPathCell
- NSPathComponentCell
- NSPathControl
- NSPopUpButton
- NSPopUpButtonCell
- NSPredicateEditor
- NSProgressIndicator
- NSRuleEditor
- NSRulerView
- NSSavePanel
- NSScrollView
- NSScroller
- NSScrubber
- NSScrubberArrangedView
- NSScrubberImageItemView
- NSScrubberItemView
- NSScrubberSelectionView
- NSScrubberTextItemView
- NSSearchField
- NSSearchFieldCell
- NSSecureTextField
- NSSecureTextFieldCell
- NSSegmentedCell
- NSSegmentedControl
- NSSlider
- NSSliderCell
- NSSplitView
- NSSplitViewController
- NSStackView
- NSStatusBarButton
- NSStepper
- NSStepperCell
- NSSwitch
- NSTabView
- NSTabViewController
- NSTableCellView
- NSTableColumn
- NSTableHeaderCell
- NSTableHeaderView
- NSTableRowView
- NSTableView
- NSText
- NSTextAttachmentCell
- NSTextField
- NSTextFieldCell
- NSTextInsertionIndicator
- NSTextView
- NSTitlebarAccessoryViewController
- NSTokenField
- NSTokenFieldCell
- NSView
- NSViewController
- NSVisualEffectView
- NSWindow

## See Also

### Window Restoration

protocol NSWindowRestoration

A set of methods that restoration classes must implement to handle the recreation of windows.

