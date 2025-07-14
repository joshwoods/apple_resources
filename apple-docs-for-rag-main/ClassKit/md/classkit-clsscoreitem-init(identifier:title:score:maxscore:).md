

- ClassKit
- CLSScoreItem
-  init(identifier:title:score:maxScore:) 

Initializer

# init(identifier:title:score:maxScore:)

Initializes an activity item that holds a score value.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
init(
    identifier: String,
    title: String,
    score: Double,
    maxScore: Double
)
```

## Parameters 

`identifier`  

A unique string identifier for the activity item.

`title`  

A human readable name for the activity item.

`score`  

The score earned during completion of a task.

`maxScore`  

The maximum possible score, against which the reported score should be judged.

