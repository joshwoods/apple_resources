

- RealityKit
- ObjectCaptureSession
-  ObjectCaptureSession.Updates 

Structure

# ObjectCaptureSession.Updates

Used to provide an `AsyncSequence` of change events for the observable properties.

RealityKitSwiftUIiOS 17.0+iPadOS 17.0+

``` source
struct Updates where Element : Sendable
```

## Topics

### Structures

struct Iterator

### Instance Methods

func makeAsyncIterator() -> ObjectCaptureSession.Updates&lt;Element>.Iterator

Creates the asynchronous iterator that produces elements of this asynchronous sequence.

### Type Aliases

typealias AsyncIterator

The type of asynchronous iterator that produces elements of this asynchronous sequence.

### Default Implementations

AsyncSequence Implementations

## Relationships

### Conforms To

- AsyncSequence
- Sendable

