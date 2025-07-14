

- AppKit
- NSWritingToolsCoordinator
-  NSWritingToolsCoordinator.TextUpdateReason 

Enumeration

# NSWritingToolsCoordinator.TextUpdateReason

Constants that specify the reason you updated your view’s content outside of the Writing Tools workflow.

macOS 15.2+

``` source
enum TextUpdateReason
```

## Overview

If you modify your view’s text storage while Writing Tools is active, report those changes to your NSWritingToolsCoordinator object so it can track them correctly. Call the updateRange(_:with:reason:forContextWithIdentifier:) method to report changes that occur inside one of your context objects. Call the updateForReflowedTextInContextWithIdentifier(_:) method for changes that affect the layout of your text, such as text insertions before a context object or changes to your view’s frame rectangle.

## Topics

### Getting the reasons

case typing

An operation that involved a person editing the text in your view.

case undoRedo

An operation that changed the view’s text as part of an undo or redo command.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Reporting changes to Writing Tools

func updateRange(NSRange, with: NSAttributedString, reason: NSWritingToolsCoordinator.TextUpdateReason, forContextWithIdentifier: UUID)

Informs the coordinator about changes your app made to the text in the specified context object.

func updateForReflowedTextInContextWithIdentifier(UUID)

Informs the coordinator that a change occurred to the view or its text that requires a layout update.

