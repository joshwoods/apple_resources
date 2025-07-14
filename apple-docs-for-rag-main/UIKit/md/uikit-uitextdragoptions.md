

- UIKit
-  UITextDragOptions 

Structure

# UITextDragOptions

A set of options that determine the behavior of a draggable text view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
struct UITextDragOptions
```

## Topics

### Text drag options

static var stripTextColorFromPreviews: UITextDragOptions

Strips the foreground and background colors for a system-provided text drag preview.

### Initializers

init(rawValue: Int)

Creates a text-drag options structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Text view additions

protocol UITextDragDelegate

The interface for customizing the behavior of a drag activity for a text view.

protocol UITextDropDelegate

The interface for configuring a text view’s drop behavior.

protocol UITextDraggable

The interface that determines if a text view is a drag source.

protocol UITextDroppable

The interface that determines if a text view is a drop destination.

enum UITextDropEditability

The text-drop editability styles for noneditable text views.

