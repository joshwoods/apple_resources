

- Create ML Components
- JointsSelector
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Select joints to be included in the pose. Ignored joints will be reset to zero in all fields.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to input: Pose,
    eventHandler: EventHandler? = nil
) -> Pose
```

## Parameters 

`input`  

A pose.

`eventHandler`  

An event handler.

## Return Value

A pose with the ignored joints set to zero.

