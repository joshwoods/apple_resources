

- MusicKit
- MusicSubscription
- MusicSubscription.Updates
-  MusicSubscription.Updates.Iterator 

Structure

# MusicSubscription.Updates.Iterator

An iterator for the asynchronous sequence to use for observing updates to the current state of the user’s subscription to Apple Music.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Iterator
```

## Topics

### Instance Methods

func next() async -> MusicSubscription?

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

### Type Aliases

typealias Element

### Default Implementations

AsyncIteratorProtocol Implementations

## Relationships

### Conforms To

- AsyncIteratorProtocol

