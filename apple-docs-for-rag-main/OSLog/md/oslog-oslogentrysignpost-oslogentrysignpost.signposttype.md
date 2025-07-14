

- OSLog
- OSLogEntrySignpost
-  OSLogEntrySignpost.SignpostType 

Enumeration

# OSLogEntrySignpost.SignpostType

The available signpost types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum SignpostType
```

## Topics

### Enumeration Cases

case undefined

The signpost does not have a type.

case intervalBegin

The signpost marks the start of a time interval.

case intervalEnd

The signpost marks the end of a time interval.

case event

The signpost marks an event.

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

### Accessing Signpost Types

var signpostType: OSLogEntrySignpost.SignpostType

The signpost’s type.

