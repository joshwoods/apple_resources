

- Foundation
- NSWhoseSpecifier
-  NSWhoseSpecifier.SubelementIdentifier 

Enumeration

# NSWhoseSpecifier.SubelementIdentifier

`NSWhoseSpecifier` uses these constants to specify sub-elements within the collection of objects being tested that pass the specifier’s test.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SubelementIdentifier
```

## Overview

These constants are used by startSubelementIdentifier, startSubelementIdentifier, endSubelementIdentifier, and endSubelementIdentifier.

## Topics

### Constants

case indexSubelement

An element at a given index that meets the specifier test.

case everySubelement

Every element that meets the specifier test.

case middleSubelement

The middle element that meets the specifier test.

case randomSubelement

Any element that meets the specifier test.

case noSubelement

No sub-element met the specifier test. Valid only for specifying the end sub-element.; that is, there is no end, so consider all elements.

case indexSubelement

An element at a given index that meets the specifier test.

case everySubelement

Every element that meets the specifier test.

case middleSubelement

The middle element that meets the specifier test.

case randomSubelement

Any element that meets the specifier test.

case noSubelement

No sub-element met the specifier test. Valid only for specifying the end sub-element.; that is, there is no end, so consider all elements.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

