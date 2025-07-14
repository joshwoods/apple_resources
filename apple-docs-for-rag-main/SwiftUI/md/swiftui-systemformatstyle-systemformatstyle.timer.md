

- SwiftUI
- SystemFormatStyle
-  SystemFormatStyle.Timer 

Structure

# SystemFormatStyle.Timer

The system timer format style.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct Timer
```

## Topics

### Initializers

init(countingDownIn: Range&lt;Date>, showsHours: Bool, maxFieldCount: Int, maxPrecision: Duration)

Create a timer format style that counts down from the given interval.

init(countingUpIn: Range&lt;Date>, showsHours: Bool, maxFieldCount: Int, maxPrecision: Duration)

Create a timer format style that counts up to the given interval.

## Relationships

### Conforms To

- Copyable
- Decodable
- DiscreteFormatStyle
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

