

- Cinematic
- CNScript
-  userDecisions(in:) 

Instance Method

# userDecisions(in:)

All user decisions in the given time range.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final func userDecisions(in timeRange: CMTimeRange) -> [CNDecision]
```

## Parameters 

`timeRange`  

The time range of interest.

## Return Value

An array of user decisions in the given time range. These include user decisions made during recording or added to the script.

