

- Shared With You
-  SWHighlightMentionEvent 

Class

# SWHighlightMentionEvent

An object that represents mention activity for a highlight.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWHighlightMentionEvent
```

## Mentioned in 

Adding custom collaboration to your app

## Topics

### Creating a mention event

init(highlight: SWHighlight, mentionedPersonCloudKitShareHandle: String)

Creates and initializes a mention event.

init(highlight: SWHighlight, mentionedPersonIdentity: SWPerson.Identity)

Creates and initializes a mention event.

### Accessing the event person

var mentionedPersonHandle: String

The handle of the person the sender mentions.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
- SWHighlightEvent

## See Also

### Highlight events

protocol SWHighlightEvent

A protocol that defines an activity that the system posts in response to a user action for a highlight.

class SWHighlightChangeEvent

An object that represents change activity for a highlight.

class SWHighlightMembershipEvent

An object that represents membership activity for a highlight.

class SWHighlightPersistenceEvent

An object that represents persistence activity for a highlight.

