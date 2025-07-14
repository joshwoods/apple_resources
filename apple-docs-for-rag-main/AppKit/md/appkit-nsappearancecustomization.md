

- AppKit
-  NSAppearanceCustomization 

Protocol

# NSAppearanceCustomization

A set of methods for getting and setting the appearance attributes of a view.

macOS

``` source
protocol NSAppearanceCustomization : NSObjectProtocol
```

## Overview

When an object adopts this protocol, assigning a value to the appearance property causes that object to use the appearance attributes you specified instead of any inherited attributes. You can access the current attributes for the object from the effectiveAppearance property, which reflects any inherited attributes.

## Topics

### Getting and Setting Appearance

Choosing a Specific Appearance for Your macOS App

Adopt a specific appearance for your windows, views, or app when it is inappropriate to support both light and dark variants.

var appearance: NSAppearance?

The appearance of the receiver, in an `NSAppearance` object.

**Required**

var effectiveAppearance: NSAppearance

The appearance that will be used when the receiver is drawn onscreen, in an `NSAppearance` object. (read-only)

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
- NSColorPanel
- NSColorWell
- NSComboBox
- NSComboButton
- NSControl
- NSDatePicker
- NSFontPanel
- NSForm
- NSGridView
- NSImageView
- NSLevelIndicator
- NSMatrix
- NSMenu
- NSOpenGLView
- NSOpenPanel
- NSOutlineView
- NSPanel
- NSPathControl
- NSPopUpButton
- NSPopover
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
- NSSecureTextField
- NSSegmentedControl
- NSSlider
- NSSplitView
- NSStackView
- NSStatusBarButton
- NSStepper
- NSSwitch
- NSTabView
- NSTableCellView
- NSTableHeaderView
- NSTableRowView
- NSTableView
- NSText
- NSTextField
- NSTextInsertionIndicator
- NSTextView
- NSTokenField
- NSView
- NSVisualEffectView
- NSWindow

## See Also

### Appearance System

class NSAppearance

An object that manages standard appearance attributes for UI elements in an app.

