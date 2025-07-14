

- Core Foundation
-  CFDateFormatterStyle 

Enumeration

# CFDateFormatterStyle

Data type for predefined date and time format styles.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CFDateFormatterStyle
```

## Overview

For possible values, see Date Formatter Styles

## Topics

### Enumeration Cases

case fullStyle

Specifies a full style with complete details, such as “Tuesday, April 12, 1952 AD” or “3:30:42pm PST”.

case longStyle

Specifies a long style, typically with full text, such as “November 23, 1937” or “3:30:32pm”.

case mediumStyle

Specifies a medium style, typically with abbreviated text, such as “Nov 23, 1937”.

case noStyle

Specifies no output.

case shortStyle

Specifies a short style, typically numeric only, such as “11/23/37” or “3:30pm”.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

