

- Shared With You
-  SWHighlightEvent 

Protocol

# SWHighlightEvent

A protocol that defines an activity that the system posts in response to a user action for a highlight.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
protocol SWHighlightEvent : NSCopying, NSSecureCoding, NSObjectProtocol
```

## Mentioned in 

Adding shared content collaboration to your app

## Topics

### Accessing the URL

var highlightURL: URL

**Required**

## Relationships

### Inherits From

- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

### Conforming Types

- SWHighlightChangeEvent
- SWHighlightMembershipEvent
- SWHighlightMentionEvent
- SWHighlightPersistenceEvent

## See Also

### Highlight events

class SWHighlightChangeEvent

An object that represents change activity for a highlight.

class SWHighlightMembershipEvent

An object that represents membership activity for a highlight.

class SWHighlightMentionEvent

An object that represents mention activity for a highlight.

class SWHighlightPersistenceEvent

An object that represents persistence activity for a highlight.

