

- ActivityKit
- ActivityContent
-  staleDate 

Instance Property

# staleDate

The date when the system considers the Live Activity to be out of date.

iOS 16.2+iPadOS 16.2+

``` source
let staleDate: Date?
```

## Mentioned in 

Displaying live data with Live Activities

## Discussion

When time reaches the configured stale date, the system considers the Live Activity out of date, and the ActivityState of the Live Activity changes to ActivityState.stale.

## See Also

### Describing a Live Activity

init(state: State, staleDate: Date?, relevanceScore: Double)

Creates the object that describes the state and configuration of a Live Activity.

let state: State

The current state of a Live Activity in its life cycle.

let relevanceScore: Double

A score you assign that determines the order in which your Live Activities appear when you start several Live Activities for your app.

