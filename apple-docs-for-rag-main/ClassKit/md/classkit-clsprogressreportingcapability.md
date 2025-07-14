

- ClassKit
-  CLSProgressReportingCapability 

Class

# CLSProgressReportingCapability

A progress reporting capability supported by a context.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
class CLSProgressReportingCapability
```

## Overview

You use activities to report metrics about a student’s progress through the task associated with a context. Every activity automatically measures time spent performing the task, but you can provide additional information, like the percentage completion, or a final score.

To help teachers understand what to expect from a context, create a set of CLSProgressReportingCapability instances — one for each kind of metric the context reports. Add the complete set to the context by calling the addProgressReportingCapabilities(_:) method.

When you create a reporting capability, include a brief description of the capability as a localized string in the details property. Schoolwork presents this to teachers to provide additional information about the metric.

## Topics

### Creating a Progress Reporting Capability

init(kind: CLSProgressReportingCapability.Kind, details: String?)

Creates a new progress reporting capability of the given type with a descriptive string.

### Characterizing the Capability

var details: String?

A description of the capability presented to teachers.

var kind: CLSProgressReportingCapability.Kind

The kind of progress reporting capability.

enum Kind

The available kinds of progress reporting that a context can perform.

## Relationships

### Inherits From

- CLSObject

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

### Indicating progress reporting capabilities

var progressReportingCapabilities: Set&lt;CLSProgressReportingCapability>

The kinds of progress reporting that the context can perform.

func addProgressReportingCapabilities(Set&lt;CLSProgressReportingCapability>)

Adds a progress reporting capability to the set of capabilities for the context.

func resetProgressReportingCapabilities()

Resets the set of capabilities for the context.

