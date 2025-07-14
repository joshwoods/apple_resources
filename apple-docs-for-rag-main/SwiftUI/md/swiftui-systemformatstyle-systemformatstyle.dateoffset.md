

- SwiftUI
- SystemFormatStyle
-  SystemFormatStyle.DateOffset 

Structure

# SystemFormatStyle.DateOffset

A system format to display the offset to a certain date.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DateOffset
```

## Topics

### Initializers

init(to: Date, allowedFields: Set&lt;Date.ComponentsFormatStyle.Field>, maxFieldCount: Int, sign: NumberFormatStyleConfiguration.SignDisplayStrategy)

Create a format style to display the offset to a certain date.

### Instance Methods

func calendar(Calendar) -> SystemFormatStyle.DateOffset

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

