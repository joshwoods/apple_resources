

- HealthKit
-  HKHeartbeatSeriesSample 

Class

# HKHeartbeatSeriesSample

A sample that represents a series of heartbeats.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
class HKHeartbeatSeriesSample
```

## Overview

Use a HKHeartbeatSeriesQuery to access the underlying heartbeat data.

The HKHeartbeatSeriesSample class is a subclass of the HKSeriesSample class. These samples are immutable; you set the sample’s properties when you build them, and they can’t change.

### Extend Heartbeat Samples

Like many HealthKit classes, you shouldn’t subclass the HKHeartbeatSeriesSample class. You may extend this class by adding metadata with custom keys to save related data used by your app.

For more information, see addMetadata(_:completion:).

## Topics

### Metadata

let HKMetadataKeyAlgorithmVersion: String

A key that indicates the version number of the algorithm used to calculate the sample’s value.

## Relationships

### Inherits From

- HKSeriesSample

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding
- Sendable

## See Also

### Series data

class HKQuantitySeriesSampleBuilder

A builder object for incrementally building a sample that contains multiple quantities.

class HKHeartbeatSeriesBuilder

A builder object for incrementally building a heartbeat series.

