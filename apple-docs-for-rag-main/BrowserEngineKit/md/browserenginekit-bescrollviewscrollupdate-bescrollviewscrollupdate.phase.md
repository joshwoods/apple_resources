

- BrowserEngineKit
- BEScrollViewScrollUpdate
-  BEScrollViewScrollUpdate.Phase 

Enumeration

# BEScrollViewScrollUpdate.Phase

The phase of a scroll update in a scroll gesture’s lifecycle.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
enum Phase
```

## Topics

### Enumeration Cases

case began

The scroll gesture began.

case cancelled

The operating system detected an event that caused it to stop tracking the scroll gesture.

case changed

The scroll gesture changed the scroll location.

case ended

The scroll gesture came to an end.

### Initializers

init?(rawValue: Int)

### Default Implementations

Equatable Implementations

RawRepresentable Implementations

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Retrieving scroll state information

var timestamp: TimeInterval

The time at which the scroll update occurred.

var phase: BEScrollViewScrollUpdate.Phase

The point in the scrolling lifecycle represented by the scroll update.

