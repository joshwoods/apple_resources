

- ARKit
- ARKitSession
- ARKitSession.Events
- ARKitSession.Events.Iterator
-  next() 

Instance Method

# next()

Returns the next element in a sequence.

visionOS 1.0+

``` source
mutating func next() async -> ARKitSession.Events.Element?
```

## Return Value

Returns an ARKitSession.Events.Element, or `nil` if there are no more elements.

