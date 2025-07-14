

- Create ML Components
-  Event 

Structure

# Event

Maintains the status of the pipeline.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
struct Event
```

## Topics

### Creating the event

init(origin: String, itemCount: Int, totalItemCount: Int?, metrics: [MetricsKey : any Sendable])

Creates an event.

### Getting the properties

var itemCount: Int

The number of items processed so far.

var metrics: [MetricsKey : any Sendable]

A dictionary of custom metrics values.

var origin: String

A description of the event’s origin.

var totalItemCount: Int?

The total number of items being processed.

### Default Implementations

CustomDebugStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- Sendable

## See Also

### Event handling

typealias EventHandler

A closure to handle processing events.

struct MetricsKey

A key that uniquely identifies a metric.

