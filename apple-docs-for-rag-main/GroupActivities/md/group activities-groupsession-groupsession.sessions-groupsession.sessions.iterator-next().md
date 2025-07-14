

- Group Activities
- GroupSession
- GroupSession.Sessions
- GroupSession.Sessions.Iterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
mutating func next() async -> GroupSession?
```

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

