

- ClassKit
- CLSProgressReportingCapability
-  CLSProgressReportingCapability.Kind 

Enumeration

# CLSProgressReportingCapability.Kind

The available kinds of progress reporting that a context can perform.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
enum Kind
```

## Overview

Use one of these values to set the kind property in each CLSProgressReportingCapability instance when constructing a set of capabilities used to configure a context. Each kind corresponds to a different metric that you provide, like a score or a progress indication.

## Topics

### Reporting Capabilities

case duration

Time spent performing the task.

case percent

The percentage of the total task that has been completed.

case binary

A binary outcome for the task, like true or false.

case quantity

A discrete value.

case score

A score.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Characterizing the Capability

var details: String?

A description of the capability presented to teachers.

var kind: CLSProgressReportingCapability.Kind

The kind of progress reporting capability.

