

- Cinematic
- CNScript
-  baseDecisions(in:) 

Instance Method

# baseDecisions(in:)

All base decisions made automatically during recording in the given time range.

iOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+

``` source
final func baseDecisions(in timeRange: CMTimeRange) -> [CNDecision]
```

## Parameters 

`timeRange`  

The time range of the base decisions.

## Return Value

An array of base decisions in a given time range. These apply if no user decision overrides them.

