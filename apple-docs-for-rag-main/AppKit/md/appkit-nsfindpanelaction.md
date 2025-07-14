

- AppKit
-  NSFindPanelAction 

Enumeration

# NSFindPanelAction

These constants define the tags for performFindPanelAction(_:).

macOS

``` source
enum NSFindPanelAction
```

## Topics

### Constants

case showFindPanel

Displays the find panel.

Deprecated

case next

Finds the next instance of the queried text.

case previous

Finds the previous instance of the queried text.

case replaceAll

Replaces all query instances within the text view.

case replace

Replaces a single query instance within the text view.

case replaceAndFind

Replaces a single query instance and finds the next.

case setFindString

Sets the query string to the current selection.

case replaceAllInSelection

Replaces all query instances within the selection.

case selectAll

Selects all query instances in the text view.

case selectAllInSelection

Selects all query instances within the selection.

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

### Constants

enum NSSelectionGranularity

These constants specify how much the text view extends the selection when the user drags the mouse. They’re used by selectionGranularity, and selectionRange(forProposedRange:granularity:):

enum NSSelectionAffinity

These constants specify the preferred direction of selection. They’re used by selectionAffinity and setSelectedRange(_:affinity:stillSelecting:).

Input Sources Locale Identifiers

Locale identifiers represent the input sources available.

Find Panel Search Metadata

In addition to communicating search strings via the find pasteboard, the standard Find panel for `NSTextView` also communicates search option metadata, including case sensitivity and substring matching options. This metadata is stored in a property list as the findPanelSearchOptions value on the global find pasteboard. As such, third party applications may store additional keys in this property list to communicate additional metadata as desired to support the various search options common to many third-party applications’ Find panels.

enum NSFindPanelSubstringMatchType

The type of substring matching used by the Find panel.

