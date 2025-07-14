

- AppKit
- Text Display
- NSTextView
-  Find Panel Search Metadata 

API Collection

# Find Panel Search Metadata

In addition to communicating search strings via the find pasteboard, the standard Find panel for `NSTextView` also communicates search option metadata, including case sensitivity and substring matching options. This metadata is stored in a property list as the findPanelSearchOptions value on the global find pasteboard. As such, third party applications may store additional keys in this property list to communicate additional metadata as desired to support the various search options common to many third-party applications’ Find panels.

## Topics

### Constants

static let findPanelSearchOptions: NSPasteboard.PasteboardType

Type for the find panel metadata property list.

static let findPanelCaseInsensitiveSearch: NSPasteboard.PasteboardType.FindPanelSearchOptionKey

A Boolean value indicating whether the search is case-insensitive.

static let findPanelSubstringMatch: NSPasteboard.PasteboardType.FindPanelSearchOptionKey

A number object containing the match type to use in the find panel.

## See Also

### Constants

enum NSSelectionGranularity

These constants specify how much the text view extends the selection when the user drags the mouse. They’re used by selectionGranularity, and selectionRange(forProposedRange:granularity:):

enum NSSelectionAffinity

These constants specify the preferred direction of selection. They’re used by selectionAffinity and setSelectedRange(_:affinity:stillSelecting:).

enum NSFindPanelAction

These constants define the tags for performFindPanelAction(_:).

Input Sources Locale Identifiers

Locale identifiers represent the input sources available.

enum NSFindPanelSubstringMatchType

The type of substring matching used by the Find panel.

