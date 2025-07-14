

- HealthKit
- HKElectrocardiogramQuery
-  HKElectrocardiogramQuery.Result 

Enumeration

# HKElectrocardiogramQuery.Result

Partial results for an electrocardiogram query.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 13.0+visionOSwatchOS 7.0+

``` source
enum Result
```

## Overview

The query returns a HKElectrocardiogramQuery.Result.measurement(_:) result for each voltage measurement, followed by a HKElectrocardiogramQuery.Result.done result.

## Topics

### Results

case measurement(HKElectrocardiogram.VoltageMeasurement)

A single voltage measurement.

case done

The query has finished returning voltage measurements.

case error(any Error)

An error occurred while accessing the voltage measurements.

## See Also

### Accessing the Results

init(electrocardiogram: HKElectrocardiogram, dataHandler: (HKElectrocardiogramQuery, HKElectrocardiogram.VoltageMeasurement?, Bool, (any Error)?) -> Void)

Creates a new electrocardiogram query object.

