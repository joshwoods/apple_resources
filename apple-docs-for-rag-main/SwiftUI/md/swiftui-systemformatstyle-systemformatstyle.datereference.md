

- SwiftUI
- SystemFormatStyle
-  SystemFormatStyle.DateReference 

Structure

# SystemFormatStyle.DateReference

A system format style to refer to a date in the most natural way.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct DateReference
```

## Overview

The reference format is designed for referring to a certain date in the most natural way possible. The concrete format depends on the distance to the date. E.g. if an event is one minute away, most people would refer to it in a relative way, e.g. the event starts “in one minute”. However, if dates are really far away, it becomes easier to refer to them in an absolute way, e.g. the original iPhone was announced in “January 2007”.

Use the style by initializing it with the date it should refer to and format it with the point of reference, usually the current time.

## Topics

### Initializers

init(to: Date, allowedFields: Set&lt;Date.RelativeFormatStyle.Field>, maxFieldCount: Int, thresholdField: Date.RelativeFormatStyle.Field)

Create a format style to refer to a date in the most natural way.

### Instance Methods

func calendar(Calendar) -> SystemFormatStyle.DateReference

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

