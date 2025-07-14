

- MetricKit
-  MXHistogram 

Class

# MXHistogram

An object representing a histogram of data values of the same type of unit.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 12.0+visionOS 1.0+

``` source
class MXHistogram where UnitType : Unit
```

## Overview

A *histogram* measures the number of times a data point for a variable falls into a specific range of possible values within a set of data. Usually, histograms are depicted as bar charts, in which each bar represents a range of values, and the height of each bar represents the number of times the value of the variable falls within a particular range. In this class, each bar is represented by a *bucket*.

A bucket holds the results for a series of measured values, such as all the events occurring between 3 and 5 seconds. MetricKit uses fixed-width buckets that are device-independent with intervals that are based on the type of metric. Use the bucketStart and bucketEnd properties to find the start and end of an interval.

The returned results contain only buckets with at least one item so bucketEnumerator may not return all intervals.

For example, if the fixed width for the time to resume the app is 10 ms, then the sequence of buckets is:

0…9 ms, 10…19 ms, 20…29 ms, etc.

If there’s data only in the 0…9 ms and 20…29 ms buckets, then the report skips the 10…19 ms bucket.

## Topics

### Reading the buckets

var bucketEnumerator: NSEnumerator

An enumerator for the buckets containing the data in the histogram.

var totalBucketCount: Int

The total number of buckets in the histogram.

class MXHistogramBucket

An object representing a bucket of data in a histogram.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Data types

class MXCallStackTree

An object representing the call stack for an exception.

class MXMetaData

An object containing system-level information about the device.

class MXAverage

A unit of measure for an average.

class MXDiagnostic

An abstract data class for a diagnostic.

class MXMetric

An abstract data class for a metric.

enum Code

Error codes for error values from app metrics.

let MXErrorDomain: String

Error domain for error values from app metrics.

struct MXError

Error domain for error handling of app metrics.

class MXCrashDiagnosticObjectiveCExceptionReason

An object that represents the exception reason for an uncaught ObjC exception.

class MXSignpostRecord

An object representing the record for a signpost interval or event.

