

- Combine
- Record
- Record.Recording
-  receive(completion:) 

Instance Method

# receive(completion:)

Add a completion to the recording.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func receive(completion: Subscribers.Completion)
```

## Discussion

A `fatalError` will be raised if more than one completion is added.

