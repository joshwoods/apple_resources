

- Combine
- Publishers
- Publishers.Multicast
-  createSubject 

Instance Property

# createSubject

A closure that returns a subject each time a subscriber attaches to the multicast publisher.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
final let createSubject: () -> SubjectType
```

## See Also

### Inspecting Publisher Properties

let upstream: Upstream

The publisher from which this publisher receives its elements.

