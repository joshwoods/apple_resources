

- Core NFC
- CardSession
-  CardSession.EventStream 

Class

# CardSession.EventStream

An asynchronous sequence of events produced by a card session.

iOS 17.4+iPadOS 17.4+

``` source
final class EventStream
```

## Overview

Get an asychronous sequence of this type from the card session’s eventStream property. Then use the Swift `for-await-in` syntax to receive and process events as the session produces them.

## Topics

### Creating an iterator

class Iterator

The iterator that produces elements of this asynchronous sequence.

## Relationships

### Conforms To

- AsyncSequence

## See Also

### Handling card events

var eventStream: CardSession.EventStream

An asynchronous sequence of events from the card session.

enum Event

A type that enumerates events produced by a card session.

