

- AppKit
-  NSCandidateListTouchBarItem 

Class

# NSCandidateListTouchBarItem

A bar item that, along with its delegate, provides a list of textual suggestions for the current text view.

macOS 10.12.2+

``` source
@MainActor
class NSCandidateListTouchBarItem where CandidateType : AnyObject
```

## Topics

### Providing a client and a delegate

var client: (any NSView &amp; NSTextInputClient)?

The client object for the candidate list item.

var delegate: (any NSCandidateListTouchBarItemDelegate)?

The delegate of the candidate list item.

protocol NSCandidateListTouchBarItemDelegate

A set of methods that a candidate list item delegate uses to enable selection state and list visibility.

### Populating the candidate list

func setCandidates([CandidateType], forSelectedRange: NSRange, in: String?)

Sets an array of candidate objects to be displayed in the candidate list bar item.

var candidates: [CandidateType]

The array of candidate objects previously set by setCandidates(_:forSelectedRange:in:).

var attributedStringForCandidate: ((CandidateType, Int) -> NSAttributedString)?

A block that converts a candidate object into an attributed string for display in the candidate list item.

var allowsTextInputContextCandidates: Bool

A Boolean value that specifies whether a candidate list item displays candidates from text input providers.

### Handling collapsible behavior

var allowsCollapsing: Bool

A Boolean value that specifies whether the item can be collapsed.

var isCollapsed: Bool

A Boolean value that controls the visibility of the candidate list.

### Managing candidate list visibility

var isCandidateListVisible: Bool

A Boolean value that represents the visibility of this item’s candidate list.

func update(withInsertionPointVisibility: Bool)

Updates the candidate list visibility configuration based on the client’s insertion point state.

### Configuring bar customization

var customizationLabel: String!

The user-visible string identifying this item during bar customization.

## Relationships

### Inherits From

- NSTouchBarItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Touch Bar items

class NSTouchBarItem

A UI control shown in the Touch Bar on supported models of MacBook Pro.

class NSColorPickerTouchBarItem

A bar item that provides a system-defined color picker.

class NSCustomTouchBarItem

A bar item that contains a responder of your choice, such as a view, a button, or a scrubber.

class NSGroupTouchBarItem

A bar item that provides a bar to contain other items.

class NSPopoverTouchBarItem

A bar item that provides a two-state control that can expand into its second state, showing the contents of a bar that it owns.

class NSSharingServicePickerTouchBarItem

A bar item that, along with its delegate, provides a list of objects eligible for sharing.

class NSSliderTouchBarItem

A bar item that provides a slider control for choosing a value in a range.

class NSStepperTouchBarItem

A bar item that provides a stepper control for incrementing or decrementing a value.

class NSUserInterfaceCompressionOptions

An object that specifies how user interface elements resize themselves when space is constrained.

class NSButtonTouchBarItem

A bar item that provides a button.

class NSPickerTouchBarItem

A bar item that provides a picker control with multiple options.

enum ControlRepresentation

Constants that specify display styles for picker bar items.

enum SelectionMode

Constants that specify selection modes for picker bar items.

