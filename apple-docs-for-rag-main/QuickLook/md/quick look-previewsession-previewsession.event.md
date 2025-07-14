

- Quick Look
- PreviewSession
-  PreviewSession.Event 

Enumeration

# PreviewSession.Event

An event from the preview session’s events stream.

visionOS 2.0+

``` source
enum Event
```

## Topics

### Enumeration Cases

case didClose

The session did close.

case didFail(any Error)

The session failed to open with an error.

case didOpen

The session did successfully open.

## Relationships

### Conforms To

- Sendable

