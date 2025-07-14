

- AppKit
- NSTextFinder
-  NSTextFinder.Action 

Enumeration

# NSTextFinder.Action

These constants specify the user interface item tags that correspond find action. These constants are passed to the performTextFinderAction(_:) method, the responder will call the appropriate method for the tag. That method will, in turn, determine the desired action and invoke the appropriate method in the `NSTextFinder` object’s `NSTextFinderClient` protocol.

macOS 10.7+

``` source
enum Action
```

## Topics

### Constants

case showFindInterface

The find bar interface is displayed.

case nextMatch

The next match, if any, is displayed.

case previousMatch

The previous match, if any, is displayed.

case replaceAll

All occurrences of the string are replaced.

case replace

Replaces a single instance of the string.

case replaceAndFind

Replaces a single instance of the string and searches for the next match.

case setSearchString

Sets the search string.

case replaceAllInSelection

Replaces all occurrences of the string within the current selection.

case selectAll

Selects all matching search strings.

case selectAllInSelection

Selects all matching search strings within the current selection.

case hideFindInterface

Hides the find bar interface.

case showReplaceInterface

Displays the find bar interface including the replace functionality.

case hideReplaceInterface

Displays the find bar interface including the replace functionality.

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

### Constants

Text Finder Options For The Pasteboard

The following keys are used for communicating `NSTextFinder` search options via pasteboard. Use the textFinderOptions type

enum MatchingType

The following constants indicate the type of search anchor an action should perform.

