

- AppKit
- Text Display
- NSText
-  Movement Codes 

API Collection

# Movement Codes

The reason for a change of editing focus among text fields.

## Overview

These constants are the possible values for the `NSTextMovement` key of the didEndEditingNotification `userInfo` dictionary. The field editor makes sure that these are the values sent when the user presses the Tab, Backtab, or Return key while editing, in essence describing why the user is leaving the field. The control then uses this information to decide where to send focus next.

## Topics

### Constants

var NSIllegalTextMovement: Int

Currently unused.

var NSReturnTextMovement: Int

The Return key was pressed.

var NSTabTextMovement: Int

The Tab key was pressed.

var NSBacktabTextMovement: Int

The Backtab (Shift-Tab) key was pressed.

var NSLeftTextMovement: Int

The left arrow key was pressed.

var NSRightTextMovement: Int

The right arrow key was pressed.

var NSUpTextMovement: Int

The up arrow key was pressed.

var NSDownTextMovement: Int

The down arrow key was pressed.

var NSCancelTextMovement: Int

The user cancelled the completion.

var NSOtherTextMovement: Int

The user performed some undefined action.

## See Also

### Constants

enum NSTextAlignment

Constants that specify text alignment.

enum NSWritingDirection

Constants that specify the writing direction.

Common Unicode Characters

