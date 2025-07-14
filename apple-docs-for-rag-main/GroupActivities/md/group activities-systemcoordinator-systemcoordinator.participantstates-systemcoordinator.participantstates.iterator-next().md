

- Group Activities
- SystemCoordinator
- SystemCoordinator.ParticipantStates
- SystemCoordinator.ParticipantStates.Iterator
-  next() 

Instance Method

# next()

Asynchronously advances to the next element and returns it, or ends the sequence if there is no next element.

visionOS 1.0+

``` source
mutating func next() async -> SystemCoordinator.ParticipantStates.Element?
```

## Return Value

The next element, if it exists, or `nil` to signal the end of the sequence.

