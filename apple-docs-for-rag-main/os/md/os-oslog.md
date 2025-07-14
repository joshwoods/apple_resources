

- os
-  OSLog 

Class

# OSLog

A container of related log messages.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
class OSLog
```

## Mentioned in 

Generating Log Messages from Your Code

## Overview

A log categorizes the messages you write and makes it easy to sort and filter them. Each log contains a subsystem and a category, which you define. A subsystem identifies a major functional area of your app, which you specify using reverse DNS notation, such as `com.your_company.your_subsystem_name`. A category segregates specific areas within a subsystem.

## Topics

### Creating a Log

convenience init(subsystem: String, category: String)

Creates a log using the specified subsystem and category.

convenience init(subsystem: String, category: OSLog.Category)

Creates a log using the specified subsystem and system-defined category.

struct Category

System-defined categories that identify well-known parts of your app.

### Getting the Shared Logs

static let `default`: OSLog

The shared default log.

static let disabled: OSLog

The shared disabled log.

### Getting Log Configuration

func isEnabled(type: OSLogType) -> Bool

Returns a Boolean value that indicates whether the log can write messages with the specified log type.

var signpostsEnabled: Bool

A Boolean value that indicates whether a log is able to use signpost logging.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Creating a Logger

init()

Creates a logger that writes to the default subsystem.

init(subsystem: String, category: String)

Creates a logger using the specified subsystem and category.

init(OSLog)

Creates a logger that writes to the specified log.

