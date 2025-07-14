

- Foundation
-  ReferenceConvertible 

Protocol

# ReferenceConvertible

A decoration applied to types that are backed by a Foundation reference type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol ReferenceConvertible : CustomDebugStringConvertible, CustomStringConvertible, Hashable, _ObjectiveCBridgeable
```

## Overview

All `ReferenceConvertible` types are hashable, equatable, and provide description functions.

Warning

Don’t create new conformances to this protocol. `ReferenceConvertible` only supports types provided by the SDK.

## Topics

### Supporting types

associatedtype ReferenceType : NSObject, NSCopying

**Required**

## Relationships

### Inherits From

- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable

### Conforming Types

- AffineTransform
- Calendar
- CharacterSet
- Data
- Date
- DateComponents
- DateInterval
- IndexPath
- IndexSet
- Locale
- Measurement
- Notification
- PersonNameComponents
- TimeZone
- URL
- URLComponents
- URLQueryItem
- URLRequest
- UUID

## See Also

### Swift Support

Classes Bridged to Swift Standard Library Value Types

Use bridged reference types when you need reference semantics or Foundation-specific behavior.

