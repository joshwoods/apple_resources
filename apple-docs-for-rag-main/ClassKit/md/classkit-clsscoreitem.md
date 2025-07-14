

- ClassKit
-  CLSScoreItem 

Class

# CLSScoreItem

Activity information that signifies a score out of a possible maximum.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
class CLSScoreItem
```

## Overview

Use an activity item of this type to indicate the relative success in completing a task, like the number of correctly answered questions on a quiz.

## Topics

### Creating Score Activity Items

init(identifier: String, title: String, score: Double, maxScore: Double)

Initializes an activity item that holds a score value.

### Managing the Score

var score: Double

The score earned by a user in completing the task.

var maxScore: Double

The maximum possible score that the user can earn on a given task.

## Relationships

### Inherits From

- CLSActivityItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Activity items

Recording additional metrics about a completed task

Add an activity item to an activity to record additional information about a student’s attempt to complete a task.

class CLSBinaryItem

Activity information that is true or false, pass or fail, yes or no.

class CLSQuantityItem

Activity information that signifies a quantity.

class CLSActivityItem

An abstract base class for gathering information about an activity.

