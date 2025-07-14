

- AppKit
-  NSStandardKeyBindingResponding 

Protocol

# NSStandardKeyBindingResponding

Methods that responder subclasses implement to support key binding commands, such as inserting tabs and newlines, or moving the insertion point.

macOS

``` source
@MainActor
protocol NSStandardKeyBindingResponding : NSObjectProtocol
```

## Overview

NSResponder doesn’t implement any of these methods. NSTextView implements a subset of them related to text editing. Your responder subclasses can implement any methods that make sense. You can create your own methods as well, but use these if the concepts map to functionality in your app. If your responder subclass is a view that’s key and uses key binding, and the user types a key sequence bound to a command not implemented in your class, nothing happens by default.

## Topics

### Responding to Key Commands

func doCommand(by: Selector)

Performs the given selector if possible.

### Inserting Content

func insertBacktab(Any?)

Inserts a backtab character.

func insertContainerBreak(Any?)

Inserts a container break, such as a new page break.

func insertDoubleQuoteIgnoringSubstitution(Any?)

Inserts a double quotation mark without substituting a curly quotation mark.

func insertLineBreak(Any?)

Inserts a line break character.

func insertNewline(Any?)

Inserts a newline character.

func insertNewlineIgnoringFieldEditor(Any?)

Inserts a newline character without invoking the field editor’s normal handling to end editing.

func insertParagraphSeparator(Any?)

Inserts a paragraph separator.

func insertSingleQuoteIgnoringSubstitution(Any?)

func insertTab(Any?)

Inserts a tab character.

func insertTabIgnoringFieldEditor(Any?)

func insertText(Any)

Inserts the text you specify.

### Deleting Content

func deleteBackward(Any?)

Deletes content moving backward from the current insertion point.

func deleteBackwardByDecomposingPreviousCharacter(Any?)

func deleteForward(Any?)

func deleteToBeginningOfLine(Any?)

Deletes content from the insertion point to the beginning of the current line.

func deleteToBeginningOfParagraph(Any?)

Deletes content from the insertion point to the beginning of the current paragraph.

func deleteToEndOfLine(Any?)

Deletes content from the insertion point to the end of the current line.

func deleteToEndOfParagraph(Any?)

Deletes content from the insertion point to the end of the current paragraph.

func deleteWordBackward(Any?)

Deletes the word preceding the current insertion point.

func deleteWordForward(Any?)

func yank(Any?)

Deletes the current selection, placing it in a temporary buffer, such as the Clipboard.

### Moving the Insertion Pointer

func moveBackward(Any?)

Moves the insertion pointer backward in the current content.

func moveDown(Any?)

Moves the insertion pointer down in the current content.

func moveForward(Any?)

Moves the insertion pointer forward in the current content.

func moveLeft(Any?)

Moves the insertion pointer left in the current content.

func moveRight(Any?)

Moves the insertion pointer right in the current content.

func moveUp(Any?)

Moves the insertion pointer up in the current content.

### Modifying the Selection

func moveBackwardAndModifySelection(Any?)

Extends the selection to include the content before the current selection.

func moveDownAndModifySelection(Any?)

Extends the selection to include the content below the current selection.

func moveForwardAndModifySelection(Any?)

Extends the selection to include the content after the current selection.

func moveLeftAndModifySelection(Any?)

Extends the selection to include the content to the left of the current selection.

func moveRightAndModifySelection(Any?)

Extends the selection to include the content to the right of the current selection.

func moveUpAndModifySelection(Any?)

Extends the selection to include the content above the current selection.

### Scrolling Content

func scrollPageDown(Any?)

Scrolls the content down by a page.

func scrollPageUp(Any?)

Scrolls the content up by a page.

func scrollLineDown(Any?)

Scrolls the content down by a line.

func scrollLineUp(Any?)

Scrolls the content up by a line.

func scrollToBeginningOfDocument(Any?)

Scrolls the content to the beginning of the document.

func scrollToEndOfDocument(Any?)

Scrolls the content to the end of the document.

func pageDown(Any?)

Moves the visible content region down by a page.

func pageUp(Any?)

Moves the visible content region up by a page.

func pageDownAndModifySelection(Any?)

Moves the visible content region down by a page, and extends the current selection.

func pageUpAndModifySelection(Any?)

Moves the visible content region up by a page, and extends the current selection.

func centerSelectionInVisibleArea(Any?)

Moves the visible content region so the current selection is visually centered.

### Transposing Elements

func transpose(Any?)

Transposes the content around the current selection.

func transposeWords(Any?)

Transposes the words around the current selection.

### Indenting Content

func indent(Any?)

Indents the content at the current selection.

### Canceling Operations

func cancelOperation(Any?)

Cancels the current operation.

### Supporting QuickLook

func quickLookPreviewItems(Any?)

Invokes QuickLook to preview the current selection.

### Supporting Writing Directions

func makeBaseWritingDirectionLeftToRight(Any?)

func makeBaseWritingDirectionNatural(Any?)

func makeBaseWritingDirectionRightToLeft(Any?)

func makeTextWritingDirectionLeftToRight(Any?)

func makeTextWritingDirectionNatural(Any?)

func makeTextWritingDirectionRightToLeft(Any?)

### Changing Capitalization

func capitalizeWord(Any?)

func changeCaseOfLetter(Any?)

func lowercaseWord(Any?)

func uppercaseWord(Any?)

### Moving the Selection in Documents

func moveToBeginningOfDocument(Any?)

func moveToBeginningOfDocumentAndModifySelection(Any?)

func moveToEndOfDocument(Any?)

func moveToEndOfDocumentAndModifySelection(Any?)

### Moving the Selection in Paragraphs

func moveParagraphBackwardAndModifySelection(Any?)

func moveParagraphForwardAndModifySelection(Any?)

func moveToBeginningOfParagraph(Any?)

func moveToBeginningOfParagraphAndModifySelection(Any?)

func moveToEndOfParagraph(Any?)

func moveToEndOfParagraphAndModifySelection(Any?)

### Moving the Selection in Lines of Text

func moveToBeginningOfLine(Any?)

func moveToBeginningOfLineAndModifySelection(Any?)

func moveToEndOfLine(Any?)

func moveToEndOfLineAndModifySelection(Any?)

func moveToLeftEndOfLine(Any?)

func moveToLeftEndOfLineAndModifySelection(Any?)

func moveToRightEndOfLine(Any?)

func moveToRightEndOfLineAndModifySelection(Any?)

### Changing the Selection

func selectAll(Any?)

func selectLine(Any?)

func selectParagraph(Any?)

func selectWord(Any?)

### Supporting Marked Selections

func setMark(Any?)

func selectToMark(Any?)

func deleteToMark(Any?)

func swapWithMark(Any?)

### Supporting Autocomplete

func complete(Any?)

### Moving the Selection by Word Boundaries

func moveWordBackward(Any?)

func moveWordBackwardAndModifySelection(Any?)

func moveWordForward(Any?)

func moveWordForwardAndModifySelection(Any?)

func moveWordLeft(Any?)

func moveWordLeftAndModifySelection(Any?)

func moveWordRight(Any?)

func moveWordRightAndModifySelection(Any?)

### Instance Methods

func showContextMenuForSelection(Any?)

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

### Responding to Action Messages

func supplementalTarget(forAction: Selector, sender: Any?) -> Any?

Finds a target for an action method.

Action Messages

Implement action messages in your first responders to handle common tasks.

