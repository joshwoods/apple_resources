

- WorkoutKit
- IntervalBlock
-  init(steps:iterations:) 

Initializer

# init(steps:iterations:)

Creates a new interval block, in which the workout repeats the provided steps the specified number of times.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
init(
    steps: [IntervalStep] = [],
    iterations: Int = 1
)
```

## Parameters 

`steps`  

A series of work and recovery steps for the interval block.

`iterations`  

The number of times the interval block repeats its steps.

