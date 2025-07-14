

- Foundation
- NSURLRequest
-  NSURLRequest.Attribution 

Enumeration

# NSURLRequest.Attribution

The entities that can make a network request.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
enum Attribution
```

## Overview

Use one of these values when setting the attribution parameter of a URLRequest. If you don’t set a value, the system assumes NSURLRequest.Attribution.developer.

## Topics

### Request sources

case developer

A developer-initiated network request.

case user

The user explicitly directs the app to make a network request.

case developer

A developer-initiated network request.

case user

The user explicitly directs the app to make a network request.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Indicating the source of the request

var attribution: NSURLRequest.Attribution

The entity that initiates the network request.

