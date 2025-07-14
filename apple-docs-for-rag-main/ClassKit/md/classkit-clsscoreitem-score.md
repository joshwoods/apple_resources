

- ClassKit
- CLSScoreItem
-  score 

Instance Property

# score

The score earned by a user in completing the task.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var score: Double { get set }
```

## Discussion

The value given here is judged against the activity item’s maxScore, so for a quiz with 8 questions, the maximum might be 8, and the score might be an integer in the range \[0, 8\].

## See Also

### Managing the Score

var maxScore: Double

The maximum possible score that the user can earn on a given task.

