

- Background Assets
- BADownload
-  BADownload.Priority 

Structure

# BADownload.Priority

A type that determines the execution priority of a scheduled asset download.

iOSiPadOSMac CatalystmacOStvOSvisionOS

``` source
struct Priority
```

## Overview

Use BADownload.Priority to assign an app-specific priority to a download or group of downloads. The system processes downloads with a higher priority before those with a lower priority, no matter what order you schedule them in.

## Topics

### Creating a priority

init(Int)

Creates a priority using the specified integer value.

init(rawValue: Int)

Creates a priority using the specified raw value.

### Getting system priorities

static let `default`: BADownload.Priority

The default execution priority.

static let min: BADownload.Priority

The lowest execution priority.

static let max: BADownload.Priority

The highest execution priority.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Asset downloads

class BAURLDownload

An object that represents a remote asset to download.

class BADownload

An object that represents an in-progress or concluded asset download.

