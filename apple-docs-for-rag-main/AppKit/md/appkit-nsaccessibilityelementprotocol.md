

- AppKit
-  NSAccessibilityElementProtocol 

Protocol

# NSAccessibilityElementProtocol

A role-based protocol that declares the minimum interface necessary to interact with an assistive app.

macOS

``` source
protocol NSAccessibilityElementProtocol : NSObjectProtocol
```

## Overview

This protocol provides the base behavior for more specific, role-based accessibility protocols. In general, your user interface elements shouldn’t adopt this protocol. They should adopt a more specific, role-based protocol instead. See Custom Controls.

Explicit Implementation Required

Any class that adopts this protocol must implement all of its methods, and the required methods of any protocol it inherits from. The compiler may require you to override some methods that your ancestors have already implemented. Simply follow the compiler’s warnings, and reimplement these methods as necessary.

## Topics

### Supporting Accessibility

func accessibilityFrame() -> NSRect

Returns the accessibility element’s frame in screen coordinates.

**Required**

func accessibilityIdentifier() -> String

Returns the accessibility element’s identity.

func accessibilityParent() -> Any?

Returns the accessibility element’s parent in the accessibility hierarchy.

**Required**

func isAccessibilityFocused() -> Bool

Returns a Boolean value that indicates whether the accessibility element has the keyboard focus.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- NSAccessibilityButton
- NSAccessibilityCheckBox
- NSAccessibilityContainsTransientUI
- NSAccessibilityGroup
- NSAccessibilityImage
- NSAccessibilityLayoutArea
- NSAccessibilityLayoutItem
- NSAccessibilityList
- NSAccessibilityNavigableStaticText
- NSAccessibilityOutline
- NSAccessibilityProgressIndicator
- NSAccessibilityRadioButton
- NSAccessibilityRow
- NSAccessibilitySlider
- NSAccessibilityStaticText
- NSAccessibilityStepper
- NSAccessibilitySwitch
- NSAccessibilityTable

### Conforming Types

- NSActionCell
- NSApplication
- NSBox
- NSBrowser
- NSBrowserCell
- NSButton
- NSButtonCell
- NSCell
- NSClipView
- NSCollectionView
- NSColorPanel
- NSColorWell
- NSComboBox
- NSComboBoxCell
- NSComboButton
- NSControl
- NSDatePicker
- NSDatePickerCell
- NSDrawer
- NSFontPanel
- NSForm
- NSFormCell
- NSGridView
- NSImageCell
- NSImageView
- NSLevelIndicator
- NSLevelIndicatorCell
- NSMatrix
- NSMenu
- NSMenuItem
- NSMenuItemCell
- NSOpenGLView
- NSOpenPanel
- NSOutlineView
- NSPanel
- NSPathCell
- NSPathComponentCell
- NSPathControl
- NSPopUpButton
- NSPopUpButtonCell
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
- NSSearchFieldCell
- NSSecureTextField
- NSSecureTextFieldCell
- NSSegmentedCell
- NSSegmentedControl
- NSSlider
- NSSliderAccessory
- NSSliderCell
- NSSplitView
- NSStackView
- NSStatusBarButton
- NSStepper
- NSStepperCell
- NSSwitch
- NSTabView
- NSTableCellView
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
- NSTokenField
- NSTokenFieldCell
- NSView
- NSVisualEffectView
- NSWindow

