

- AppKit
-  NSUserActivityRestoring 

Protocol

# NSUserActivityRestoring

A protocol that marks classes to restore the state of your app to continue a user activity.

macOS

``` source
protocol NSUserActivityRestoring : NSObjectProtocol
```

## Overview

Don’t conform your classes to NSUserActivityRestoring, as it’s a marker protocol adopted by NSResponder and NSDocument for user activity state restoration.

## Topics

### Restoring App State

func restoreUserActivityState(NSUserActivity)

Restores the state necessary to continue the specified user activity.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSApplication
- NSBox
- NSBrowser
- NSButton
- NSClipView
- NSCollectionView
- NSCollectionViewItem
- NSColorPanel
- NSColorWell
- NSComboBox
- NSComboButton
- NSControl
- NSDatePicker
- NSDocument
- NSDrawer
- NSFontPanel
- NSForm
- NSGridView
- NSImageView
- NSLevelIndicator
- NSMatrix
- NSOpenGLView
- NSOpenPanel
- NSOutlineView
- NSPageController
- NSPanel
- NSPathControl
- NSPersistentDocument
- NSPopUpButton
- NSPopover
- NSPredicateEditor
- NSProgressIndicator
- NSResponder
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
- NSSecureTextField
- NSSegmentedControl
- NSSlider
- NSSplitView
- NSSplitViewController
- NSStackView
- NSStatusBarButton
- NSStepper
- NSSwitch
- NSTabView
- NSTabViewController
- NSTableCellView
- NSTableHeaderView
- NSTableRowView
- NSTableView
- NSText
- NSTextField
- NSTextInsertionIndicator
- NSTextView
- NSTitlebarAccessoryViewController
- NSTokenField
- NSView
- NSViewController
- NSVisualEffectView
- NSWindow
- NSWindowController

## See Also

### Handoff

class NSUserActivity

A representation of the state of your app at a moment in time.

