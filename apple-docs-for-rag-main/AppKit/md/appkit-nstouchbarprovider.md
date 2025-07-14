

- AppKit
-  NSTouchBarProvider 

Protocol

# NSTouchBarProvider

A protocol that an object adopts to create a bar object in your app.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS

``` source
protocol NSTouchBarProvider : NSObjectProtocol
```

## Topics

### Providing a Touch Bar

var touchBar: NSTouchBar?

The property you implement to provide a Touch Bar object.

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

### Essentials

Integrating a Toolbar and Touch Bar into Your App

Provide users quick access to your app’s features from a toolbar and corresponding Touch Bar.

Creating and Customizing the Touch Bar

Adopt Touch Bar support by displaying interactive content and controls for your macOS apps.

class NSTouchBar

An object that provides dynamic contextual controls in the Touch Bar of supported models of MacBook Pro.

protocol NSTouchBarDelegate

A protocol that allows you to provide the items for a bar dynamically.

