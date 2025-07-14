

- Cinematic
- CNScript
-  decision(after:) 

Instance Method

# decision(after:)

The decision that occurs after the given time.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final func decision(after time: CMTime) -> CNDecision?
```

## Parameters 

`time`  

The time of the decision to occur after.

## Return Value

The decision that occurred after the given time.

## Discussion

Pass the time of an existing decision to find the next one.

