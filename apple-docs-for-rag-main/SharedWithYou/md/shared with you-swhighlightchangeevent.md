

- Shared With You
-  SWHighlightChangeEvent 

Class

# SWHighlightChangeEvent

An object that represents change activity for a highlight.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class SWHighlightChangeEvent
```

## Mentioned in 

Adding shared content collaboration to your app

## Topics

### Creating a change event

init(highlight: SWHighlight, trigger: SWHighlightChangeEventTrigger)

Creates and initializes a change event.

### Accessing event attributes

var highlightURL: URL

The URL of the hightlight.

var changeEventTrigger: SWHighlightChangeEventTrigger

The type of change event for the highlight.

enum SWHighlightChangeEventTrigger

The type of change event for the highlight

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

class SWHighlightMembershipEvent

An object that represents membership activity for a highlight.

class SWHighlightMentionEvent

An object that represents mention activity for a highlight.

class SWHighlightPersistenceEvent

An object that represents persistence activity for a highlight.

