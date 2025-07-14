

- os
- OSSignpostIntervalState
-  beginState(id:) 

Type Method

# beginState(id:)

Recreates interval state from the specified signpost ID.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
static func beginState(id: OSSignpostID) -> OSSignpostIntervalState
```

## Parameters 

`id`  

The signpost ID you use to begin the signposted interval.

## Return Value

The recreated interval state.

## Discussion

Important

Recreating interval state to end a signposted interval bypasses runtime assertions that check for consistency between the beginning and the end of the interval.

