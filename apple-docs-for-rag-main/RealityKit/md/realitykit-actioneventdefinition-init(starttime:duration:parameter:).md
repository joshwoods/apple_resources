

- RealityKit
- ActionEventDefinition
-  init(startTime:duration:parameter:) 

Initializer

# init(startTime:duration:parameter:)

Constructs an event definition.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    startTime: TimeInterval,
    duration: TimeInterval,
    parameter: ActionEventDefinition.EventParameterType? = nil
)
```

## Parameters 

`startTime`  

The time when the event becomes active.

`duration`  

The duration of the event.

`parameter`  

The event parameter to return to the event handler when the event occurs.

