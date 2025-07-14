

- Cinematic
- CNScript
-  frame(at:tolerance:) 

Instance Method

# frame(at:tolerance:)

The closest frame to the given time within the given tolerance.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final func frame(
    at time: CMTime,
    tolerance: CMTime
) -> CNScript.Frame?
```

## Parameters 

`time`  

The time of interest.

`tolerance`  

The tolerance time.

## Return Value

The closest frame to the time of interest within the given tolerance.

