

- Foundation
- Formatter
-  Formatter.UnitStyle 

Enumeration

# Formatter.UnitStyle

Specifies the width of the unit, determining the textual representation.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum UnitStyle
```

## Overview

The unit is represented in the shortest notation available. For example, for English, when formatting “3 pounds”: Formatter.UnitStyle.long is “3 pounds”; Formatter.UnitStyle.medium is “3 lb”; Formatter.UnitStyle.short is “3#”.

## Topics

### Constants

case short

Specifies a short unit style.

case medium

Specifies a medium unit style.

case long

Specifies a long unit style.

case short

Specifies a short unit style.

case medium

Specifies a medium unit style.

case long

Specifies a long unit style.

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

### Constants

enum Context

The formatting context for a formatter.

