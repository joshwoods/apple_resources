

- WorkoutKit
- IntervalStep
-  IntervalStep.Purpose 

Enumeration

# IntervalStep.Purpose

An interval step’s purpose.

iOS 17.0+iPadOS 17.0+Mac Catalyst 18.0+macOS 15.0+watchOS 10.0+

``` source
enum Purpose
```

## Topics

### Determining the purpose

case recovery

A recovery step.

case work

A work step.

### Comparing purposes

var hashValue: Int

func hash(into: inout Hasher)

static func != (Self, Self) -> Bool

static func == (IntervalStep.Purpose, IntervalStep.Purpose) -> Bool

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

