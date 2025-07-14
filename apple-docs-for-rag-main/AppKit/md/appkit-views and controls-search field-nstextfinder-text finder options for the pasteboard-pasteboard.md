

- AppKit
- Views and Controls
- Search Field
- NSTextFinder
-  Text Finder Options For The Pasteboard 

API Collection

# Text Finder Options For The Pasteboard

The following keys are used for communicating `NSTextFinder` search options via pasteboard. Use the textFinderOptions type

## Topics

### Constants

static let textFinderCaseInsensitiveKey: NSPasteboard.PasteboardType.TextFinderOptionKey

A Boolean value indicating whether the search is case insensitive.

static let textFinderMatchingTypeKey: NSPasteboard.PasteboardType.TextFinderOptionKey

A number object containing the match type to use.

## See Also

### Constants

enum Action

These constants specify the user interface item tags that correspond find action. These constants are passed to the performTextFinderAction(_:) method, the responder will call the appropriate method for the tag. That method will, in turn, determine the desired action and invoke the appropriate method in the `NSTextFinder` object’s `NSTextFinderClient` protocol.

enum MatchingType

The following constants indicate the type of search anchor an action should perform.

