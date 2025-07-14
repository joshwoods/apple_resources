

- Create ML Components
- PoseSelector
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Select a pose if multiple poses are detected on the same frame.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to input: [Pose],
    eventHandler: EventHandler? = nil
) -> Pose
```

## Parameters 

`input`  

An array of poses.

`eventHandler`  

An event handler.

## Return Value

A selected pose based on the strategy.

