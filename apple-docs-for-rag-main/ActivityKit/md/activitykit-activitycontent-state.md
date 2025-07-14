

- ActivityKit
- ActivityContent
-  state 

Instance Property

# state

The current state of a Live Activity in its life cycle.

iOS 16.2+iPadOS 16.2+

``` source
let state: State
```

## Discussion

This value is the same as activityState.

## See Also

### Describing a Live Activity

init(state: State, staleDate: Date?, relevanceScore: Double)

Creates the object that describes the state and configuration of a Live Activity.

let staleDate: Date?

The date when the system considers the Live Activity to be out of date.

let relevanceScore: Double

A score you assign that determines the order in which your Live Activities appear when you start several Live Activities for your app.

