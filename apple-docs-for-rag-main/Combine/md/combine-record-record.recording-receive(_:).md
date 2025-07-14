

- Combine
- Record
- Record.Recording
-  receive(\_:) 

Instance Method

# receive(\_:)

Add an output to the recording.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
mutating func receive(_ input: Record.Recording.Input)
```

## Discussion

A `fatalError` will be raised if output is added after adding completion.

