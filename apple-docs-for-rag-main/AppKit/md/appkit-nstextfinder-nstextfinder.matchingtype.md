

- AppKit
- NSTextFinder
-  NSTextFinder.MatchingType 

Enumeration

# NSTextFinder.MatchingType

The following constants indicate the type of search anchor an action should perform.

macOS 10.7+

``` source
enum MatchingType
```

## Topics

### Constants

case contains

The match contains the string.

case startsWith

The match begins with the string.

case fullWord

The match exactly matches the string.

case endsWith

The match ends with the string.

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

enum Action

These constants specify the user interface item tags that correspond find action. These constants are passed to the performTextFinderAction(_:) method, the responder will call the appropriate method for the tag. That method will, in turn, determine the desired action and invoke the appropriate method in the `NSTextFinder` object’s `NSTextFinderClient` protocol.

Text Finder Options For The Pasteboard

The following keys are used for communicating `NSTextFinder` search options via pasteboard. Use the textFinderOptions type

