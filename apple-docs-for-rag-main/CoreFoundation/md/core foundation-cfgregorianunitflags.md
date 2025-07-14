

- Core Foundation
-  CFGregorianUnitFlags 

Structure

# CFGregorianUnitFlags

These option flags are used as a mask to indicate a specific set of fields in the CFGregorianDate or CFGregorianUnits structures.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFGregorianUnitFlags
```

## Overview

These flags are used with functions such as CFGregorianDateIsValid(_:_:) and CFAbsoluteTimeGetDifferenceAsGregorianUnits(_:_:_:_:) which operate on a CFGregorianDate or CFGregorianUnits structure. For more details, see the discussion of those functions.

## Topics

### Constants

static var unitsYears: CFGregorianUnitFlags

Specifies the year field.

Deprecated

static var unitsMonths: CFGregorianUnitFlags

Specifies the month field.

Deprecated

static var unitsDays: CFGregorianUnitFlags

Specifies the day field.

Deprecated

static var unitsHours: CFGregorianUnitFlags

Specifies the hours field.

Deprecated

static var unitsMinutes: CFGregorianUnitFlags

Specifies the minutes field.

Deprecated

static var unitsSeconds: CFGregorianUnitFlags

Specifies the seconds field.

Deprecated

static var allUnits: CFGregorianUnitFlags

Specifies all fields.

Deprecated

### Initializers

init(rawValue: CFOptionFlags)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Constants

Predefined Time Interval Values

Time intervals between the absolute reference date and certain other dates.

