

- Foundation
-  LengthFormatter 

Class

# LengthFormatter

A formatter that provides localized descriptions of linear distances, such as length and height measurements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class LengthFormatter
```

## Overview

Note

As of iOS 10, macOS 10.12, tvOS 10, and watchOS 3, Foundation provides the MeasurementFormatter class, which can be used to represent quantities of UnitLength to provide equivalent functionality to LengthFormatter. You are encouraged to transition to these new Foundation Units and Measurements APIs whenever possible.

## Topics

### Formatting Length Strings

var isForPersonHeightUse: Bool

A Boolean value that indicates whether the resulting string represents a person’s height.

func getObjectValue(AutoreleasingUnsafeMutablePointer&lt;AnyObject?>?, for: String, errorDescription: AutoreleasingUnsafeMutablePointer&lt;NSString?>?) -> Bool

This method is not supported for the `NSLengthFormatter` class.

var numberFormatter: NumberFormatter!

The number formatter used to format the numbers in length strings.

func string(fromMeters: Double) -> String

Returns a length string for the provided value.

func string(fromValue: Double, unit: LengthFormatter.Unit) -> String

Returns a properly formatted length string for the given value and unit.

func unitString(fromMeters: Double, usedUnit: UnsafeMutablePointer&lt;LengthFormatter.Unit>?) -> String

Returns the unit string for the provided value.

func unitString(fromValue: Double, unit: LengthFormatter.Unit) -> String

Returns the unit string based on the provided value and unit.

var unitStyle: Formatter.UnitStyle

The unit style used by this formatter.

### Constants

enum Unit

The units supported by the `NSLengthFormatter` class.

## Relationships

### Inherits From

- Formatter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol

## See Also

### Deprecated

class MassFormatter

A formatter that provides localized descriptions of mass and weight values.

class EnergyFormatter

A formatter that provides localized descriptions of energy values.

