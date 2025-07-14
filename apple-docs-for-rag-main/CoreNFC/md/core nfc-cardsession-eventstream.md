

- Core NFC
- CardSession
-  eventStream 

Instance Property

# eventStream

An asynchronous sequence of events from the card session.

iOS 17.4+iPadOS 17.4+

``` source
var eventStream: CardSession.EventStream { get }
```

## Discussion

Use the Swift `for-await-in` syntax to receive and process events as the session produces them.

## See Also

### Handling card events

class EventStream

An asynchronous sequence of events produced by a card session.

enum Event

A type that enumerates events produced by a card session.

