

- Combine
- Record
-  Record.Recording 

Structure

# Record.Recording

A recorded sequence of outputs, followed by a completion value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
struct Recording
```

## Topics

### Initializers

init()

Set up a recording in a state ready to receive output.

init(output: [Output], completion: Subscribers.Completion&lt;Failure>)

Set up a complete recording with the specified output and completion.

### Instance Properties

var completion: Subscribers.Completion&lt;Failure>

The completion which will be sent to a `Subscriber`.

var output: [Output]

The output which will be sent to a `Subscriber`.

### Instance Methods

func encode(into: any Encoder) throws

func receive(Record&lt;Output, Failure>.Recording.Input)

Add an output to the recording.

func receive(completion: Subscribers.Completion&lt;Failure>)

Add a completion to the recording.

### Type Aliases

typealias Input

### Default Implementations

Decodable Implementations

Encodable Implementations

## Relationships

### Conforms To

- Copyable
- Decodable
- Encodable

