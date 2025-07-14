

- Shared With You
-  SWHighlightPersistenceEvent 

Class

# SWHighlightPersistenceEvent

An object that represents persistence activity for a highlight.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWHighlightPersistenceEvent
```

## Mentioned in 

Adding shared content collaboration to your app

## Topics

### Creating a persistence event

init(highlight: SWHighlight, trigger: SWHighlightPersistenceEventTrigger)

Creates and initializes a persistence event.

### Accessing an event trigger

var persistenceEventTrigger: SWHighlightPersistenceEventTrigger

The persistence event trigger for the highlight.

enum SWHighlightPersistenceEventTrigger

Signifies the type of persistence event trigger.

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

class SWHighlightMentionEvent

An object that represents mention activity for a highlight.

