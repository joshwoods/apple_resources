

- ActivityKit
- ActivityContent
-  init(state:staleDate:relevanceScore:) 

Initializer

# init(state:staleDate:relevanceScore:)

Creates the object that describes the state and configuration of a Live Activity.

iOS 16.2+iPadOS 16.2+

``` source
init(
    state: State,
    staleDate: Date?,
    relevanceScore: Double = 0.0
)
```

## See Also

### Describing a Live Activity

let state: State

The current state of a Live Activity in its life cycle.

let staleDate: Date?

The date when the system considers the Live Activity to be out of date.

let relevanceScore: Double

A score you assign that determines the order in which your Live Activities appear when you start several Live Activities for your app.

