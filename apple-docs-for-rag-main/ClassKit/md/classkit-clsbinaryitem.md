

- ClassKit
-  CLSBinaryItem 

Class

# CLSBinaryItem

Activity information that is true or false, pass or fail, yes or no.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
class CLSBinaryItem
```

## Overview

Use an activity item of this type to indicate a binary condition, such as whether a student passed a test or failed it. Set the valueType property to specify how the binary condition should be reported to a teacher.

## Topics

### Creating Binary Activity Items

init(identifier: String, title: String, type: CLSBinaryValueType)

Initializes a new binary activity item of the given type.

enum CLSBinaryValueType

The kinds of outcomes that a binary activity item can represent.

### Managing the Value

var value: Bool

The value that the binary activity item takes.

var valueType: CLSBinaryValueType

The kind of outcome that the binary activity item represents.

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

class CLSQuantityItem

Activity information that signifies a quantity.

class CLSActivityItem

An abstract base class for gathering information about an activity.

