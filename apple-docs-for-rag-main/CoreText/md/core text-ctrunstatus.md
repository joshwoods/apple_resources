

- Core Text
-  CTRunStatus 

Structure

# CTRunStatus

A bitfield that represents the disposition of the run.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CTRunStatus
```

## Overview

The CTRunGetStatus(_:) function passes back this bitfield to indicate the disposition of the run.

## Topics

### Constants

static var rightToLeft: CTRunStatus

The run proceeds from right to left.

static var nonMonotonic: CTRunStatus

The run isn’t in strictly increasing or decreasing order.

static var hasNonIdentityMatrix: CTRunStatus

The run requires a specific text matrix to be set in the current Core Graphics context for proper drawing.

### Initializers

init(rawValue: UInt32)

Creates a run status structure with the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

