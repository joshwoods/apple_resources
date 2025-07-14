

- ClassKit
-  CLSQuantityItem 

Class

# CLSQuantityItem

Activity information that signifies a quantity.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
class CLSQuantityItem
```

## Overview

Use an activity item of this type to associate a discrete value with a task. For example, you might use it to indicate how many times the user requested a hint while taking a quiz.

## Topics

### Creating Quantity Activity Items

init(identifier: String, title: String)

Initializes an activity item that records a discrete quantity.

### Managing the Quantity

var quantity: Double

A quantity associated with the task.

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

class CLSScoreItem

Activity information that signifies a score out of a possible maximum.

class CLSBinaryItem

Activity information that is true or false, pass or fail, yes or no.

class CLSActivityItem

An abstract base class for gathering information about an activity.

