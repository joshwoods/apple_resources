

- SensorKit
-  SRFetchResult 

Class

# SRFetchResult

Recorded data that a sensor reader fetches.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
class SRFetchResult where SampleType : AnyObject
```

## Overview

A sensor reader’s delegate receives instances of this class from the sensorReader(_:didCompleteFetch:) when a fetch request finishes successfully.

Results are in the form of samples, which are of varying types depending on the reader’s sensor. For a list of sample types per sensor, see Sample types.

## Topics

### Sampling Data

var sample: SampleType

A recording that the sensor reader fetches.

var timestamp: SRAbsoluteTime

The time when the framework records the sample.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Querying data

class SRFetchRequest

An object that defines the criteria for a sample query.

