

- Quick Look
-  PreviewSession 

Structure

# PreviewSession

A structure with which you can control an existing session and receive events for the current preview application.

visionOS 2.0+

``` source
struct PreviewSession
```

## Topics

### Instance Properties

var events: some AsyncSequence&lt;PreviewSession.Event, Never>

An async sequence of preview session events.

### Instance Methods

func close() async throws

Closes the preview session.

### Enumerations

enum Event

An event from the preview session’s events stream.

## Relationships

### Conforms To

- Sendable

