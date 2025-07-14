

- Cinematic
- CNScript
-  decision(at:tolerance:) 

Instance Method

# decision(at:tolerance:)

The closest decision to the given time within the given tolerance.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final func decision(
    at time: CMTime,
    tolerance: CMTime
) -> CNDecision?
```

## Parameters 

`time`  

The time of the decision.

`tolerance`  

The tolerance time.

## Return Value

A decision representing the closest decision to the given time within the given tolerance. Returns nil if there are none.

