

- AppKit
-  NSDraggingDestination 

Protocol

# NSDraggingDestination

A set of methods that the destination object (or recipient) of a dragged image must implement.

macOS

``` source
protocol NSDraggingDestination : NSObjectProtocol
```

## Overview

The destination automatically receives NSDraggingDestination messages for pasteboard data types it has registered for as an image enters, moves around inside, and then exits or is released within the destination’s boundaries.

In macOS 10.7 and later NSDraggingDestination is a formal protocol with an updated interface. The OS X v10.6 behavior has been retained, but will be dropped in a future version of the operating system. The methods that are to be deprecated are marked as such.

## Topics

### Managing a Dragging Session Before an Image Is Released

func draggingEntered(any NSDraggingInfo) -> NSDragOperation

Invoked when the dragged image enters destination bounds or frame; delegate returns dragging operation to perform.

func wantsPeriodicDraggingUpdates() -> Bool

Asks the destination object whether it wants to receive periodic draggingUpdated(_:) messages.

func draggingUpdated(any NSDraggingInfo) -> NSDragOperation

Invoked periodically as the image is held within the destination area, allowing modification of the dragging operation or mouse-pointer position.

func draggingExited((any NSDraggingInfo)?)

Invoked when the dragged image exits the destination’s bounds rectangle (in the case of a view object) or its frame rectangle (in the case of a window object).

func draggingEnded(any NSDraggingInfo)

Called when a drag operation ends.

### Managing a Dragging Session After an Image Is Released

func prepareForDragOperation(any NSDraggingInfo) -> Bool

Invoked when the image is released, allowing the receiver to agree to or refuse drag operation.

func performDragOperation(any NSDraggingInfo) -> Bool

Invoked after the released image has been removed from the screen, signaling the receiver to import the pasteboard data.

func concludeDragOperation((any NSDraggingInfo)?)

Invoked when the dragging operation is complete, signaling the receiver to perform any necessary clean-up.

### Updating Dragging Images

func updateDraggingItemsForDrag((any NSDraggingInfo)?)

Invoked when the dragging images should be changed.

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSBox
- NSBrowser
- NSButton
- NSClipView
- NSCollectionView
- NSColorWell
- NSComboBox
- NSComboButton
- NSControl
- NSDatePicker
- NSForm
- NSGridView
- NSImageView
- NSLevelIndicator
- NSMatrix
- NSOpenGLView
- NSOutlineView
- NSPathControl
- NSPopUpButton
- NSPredicateEditor
- NSProgressIndicator
- NSRuleEditor
- NSRulerView
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

## See Also

### Drop Targets

protocol NSDraggingInfo

A set of methods that supply information about a dragging session.

protocol NSSpringLoadingDestination

A set of methods that the destination object (or recipient) of a dragged object can implement to support spring-loading.

