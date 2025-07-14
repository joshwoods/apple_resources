

- Shared With You
-  SWHighlightMembershipEvent 

Class

# SWHighlightMembershipEvent

An object that represents membership activity for a highlight.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWHighlightMembershipEvent
```

## Mentioned in 

Adding shared content collaboration to your app

## Topics

### Creating a membership event

init(highlight: SWHighlight, trigger: SWHighlightMembershipEventTrigger)

Creates and initializes a membership event.

### Accessing an event trigger

var membershipEventTrigger: SWHighlightMembershipEventTrigger

The type of membership event for the highlight.

enum SWHighlightMembershipEventTrigger

The type of membership event for the highlight.

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

class SWHighlightMentionEvent

An object that represents mention activity for a highlight.

class SWHighlightPersistenceEvent

An object that represents persistence activity for a highlight.

