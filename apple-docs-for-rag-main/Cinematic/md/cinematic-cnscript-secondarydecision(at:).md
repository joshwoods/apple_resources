

- Cinematic
- CNScript
-  secondaryDecision(at:) 

Instance Method

# secondaryDecision(at:)

If a given time is during a focus transition, the system transitions toward a secondary decision.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final func secondaryDecision(at time: CMTime) -> CNDecision?
```

## Parameters 

`time`  

The time of the focus transition.

## Return Value

The secondary decision the system is transitioning toward for the given time.

