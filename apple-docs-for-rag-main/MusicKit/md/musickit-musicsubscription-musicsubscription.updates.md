

- MusicKit
- MusicSubscription
-  MusicSubscription.Updates 

Structure

# MusicSubscription.Updates

An asynchronous sequence to use for observing updates to the current state of the user’s subscription to Apple Music.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Updates
```

## Topics

### Structures

struct Iterator

An iterator for the asynchronous sequence to use for observing updates to the current state of the user’s subscription to Apple Music.

### Instance Methods

func makeAsyncIterator() -> MusicSubscription.Updates.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

typealias Element

The type of element the asynchronous sequence produces.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence

