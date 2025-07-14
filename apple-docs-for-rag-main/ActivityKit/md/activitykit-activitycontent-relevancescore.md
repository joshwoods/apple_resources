

- ActivityKit
- ActivityContent
-  relevanceScore 

Instance Property

# relevanceScore

A score you assign that determines the order in which your Live Activities appear when you start several Live Activities for your app.

iOS 16.2+iPadOS 16.2+

``` source
let relevanceScore: Double
```

## Mentioned in 

Displaying live data with Live Activities

## Discussion

If you start more than one Live Activity in your app, the Live Activity with the highest relevance score appears in the Dynamic Island. If Live Activities have the same relevance score, the system displays the Live Activity that started first. Additionally, the `relevanceScore` determines the order of your Live Activities on the Lock Screen.

## See Also

### Describing a Live Activity

init(state: State, staleDate: Date?, relevanceScore: Double)

Creates the object that describes the state and configuration of a Live Activity.

let state: State

The current state of a Live Activity in its life cycle.

let staleDate: Date?

The date when the system considers the Live Activity to be out of date.

