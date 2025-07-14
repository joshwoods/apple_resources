

- EventKit
-  EKSourceType 

Enumeration

# EKSourceType

The type of source object.

iOSiPadOSMac CatalystmacOSvisionOSwatchOS

``` source
enum EKSourceType
```

## Overview

The sourceType property will be set to one of these values.

## Topics

### EventKit Source Types

case local

Represents a local source.

case exchange

Represents an Exchange source.

case calDAV

Represents a CalDAV or iCloud source.

case mobileMe

Represents a MobileMe source.

case subscribed

Represents a subscribed source.

case birthdays

Represents a birthday source.

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

### Accessing Source Properties

var sourceIdentifier: String

A unique identifier for the source object.

var sourceType: EKSourceType

The type of this source object.

var title: String

The name of this source object.

