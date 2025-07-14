

- os
- OSLog
-  OSLog.Category 

Structure

# OSLog.Category

System-defined categories that identify well-known parts of your app.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOSwatchOS 5.0+

``` source
struct Category
```

## Topics

### Logging Signposts

static let pointsOfInterest: OSLog.Category

The category you use to log signposts.

static let dynamicStackTracing: OSLog.Category

The category for dynamic stack tracing.

static let dynamicTracing: OSLog.Category

The category for dynamic tracing.

### Inspecting Log Categories

let rawValue: String

A string that uniquely identifies a logging category.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a Log

convenience init(subsystem: String, category: String)

Creates a log using the specified subsystem and category.

convenience init(subsystem: String, category: OSLog.Category)

Creates a log using the specified subsystem and system-defined category.

