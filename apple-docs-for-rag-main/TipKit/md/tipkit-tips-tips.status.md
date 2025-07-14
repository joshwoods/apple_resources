

- TipKit
- Tips
-  Tips.Status 

Enumeration

# Tips.Status

A type that describes the current display eligibility status for a tip.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
enum Status
```

## Topics

### Enumeration Cases

case available

The tip is eligible for display.

case invalidated(Tips.InvalidationReason)

The tip is no longer valid.

case pending

The tip is not eligible for display.

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

