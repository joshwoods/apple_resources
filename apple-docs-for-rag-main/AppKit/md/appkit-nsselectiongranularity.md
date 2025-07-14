

- AppKit
-  NSSelectionGranularity 

Enumeration

# NSSelectionGranularity

These constants specify how much the text view extends the selection when the user drags the mouse. They’re used by selectionGranularity, and selectionRange(forProposedRange:granularity:):

macOS

``` source
enum NSSelectionGranularity
```

## Topics

### Constants

case selectByCharacter

Extends the selection character by character.

case selectByWord

Extends the selection word by word.

case selectByParagraph

Extends the selection paragraph by paragraph.

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

enum NSSelectionAffinity

These constants specify the preferred direction of selection. They’re used by selectionAffinity and setSelectedRange(_:affinity:stillSelecting:).

enum NSFindPanelAction

These constants define the tags for performFindPanelAction(_:).

Input Sources Locale Identifiers

Locale identifiers represent the input sources available.

Find Panel Search Metadata

In addition to communicating search strings via the find pasteboard, the standard Find panel for `NSTextView` also communicates search option metadata, including case sensitivity and substring matching options. This metadata is stored in a property list as the findPanelSearchOptions value on the global find pasteboard. As such, third party applications may store additional keys in this property list to communicate additional metadata as desired to support the various search options common to many third-party applications’ Find panels.

enum NSFindPanelSubstringMatchType

The type of substring matching used by the Find panel.

