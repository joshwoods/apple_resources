

- Combine
- Publishers
- Publishers.Multicast
-  init(upstream:createSubject:) 

Initializer

# init(upstream:createSubject:)

Creates a multicast publisher that applies a closure to create a subject that delivers elements to subscribers.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    upstream: Upstream,
    createSubject: @escaping () -> SubjectType
)
```

## Parameters 

`createSubject`  

A closure that returns a Subject each time a subscriber attaches to the multicast publisher.

