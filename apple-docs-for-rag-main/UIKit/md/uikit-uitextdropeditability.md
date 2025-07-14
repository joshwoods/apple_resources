

- UIKit
-  UITextDropEditability 

Enumeration

# UITextDropEditability

The text-drop editability styles for noneditable text views.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum UITextDropEditability
```

## Topics

### Editability styles

case no

A text-drop editability specifier indicating that a noneditable text view does not accept drops.

case temporary

A text-drop editability specifier indicating that a noneditable text view does accept drops but reverts to its noneditable status immediately afterward.

case yes

A text-drop editability specifier indicating that a noneditable text view does accept drops, and that the dropped text remains editable after the drop is finished.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Text view additions

protocol UITextDragDelegate

The interface for customizing the behavior of a drag activity for a text view.

protocol UITextDropDelegate

The interface for configuring a text view’s drop behavior.

protocol UITextDraggable

The interface that determines if a text view is a drag source.

struct UITextDragOptions

A set of options that determine the behavior of a draggable text view.

protocol UITextDroppable

The interface that determines if a text view is a drop destination.

