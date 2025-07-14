

- Security
-  SecRequirementType 

Enumeration

# SecRequirementType

An enumeration indicating different types of internal requirements for code.

Mac Catalyst 13.0+macOS 10.0+

``` source
enum SecRequirementType
```

## Overview

These constants are indexes into requirement sets and are not currently used in any public API.

## Topics

### Constants

case hostRequirementType

What hosts may run this code.

case guestRequirementType

What guests this code may run.

case designatedRequirementType

A designated requirement.

case libraryRequirementType

What libraries this code may link against.

case pluginRequirementType

What plug-ins this code may load.

case invalidRequirementType

Invalid type of requirement.

static var requirementTypeCount: SecRequirementType

The number of valid requirement types.

### Initializers

init?(rawValue: UInt32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

