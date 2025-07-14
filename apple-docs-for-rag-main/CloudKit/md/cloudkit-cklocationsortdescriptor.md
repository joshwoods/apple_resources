

- CloudKit
-  CKLocationSortDescriptor 

Class

# CKLocationSortDescriptor

An object for sorting records that contain location data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 3.0+

``` source
class CKLocationSortDescriptor
```

## Overview

You can add a location sort descriptor to your queries when searching for records. At creation time, you must provide the sort descriptor with a key that has a CLLocation object as its value. The sort descriptor uses the value of that key to perform the sort.

CloudKit computes distance by drawing a direct line between the two locations that follows the curvature of the Earth. Distances don’t account for altitude changes between the two locations.

## Topics

### Creating a Location Sort Descriptor

init(key: String, relativeLocation: CLLocation)

Creates a location sort descriptor using the specified key and relative location.

init(coder: NSCoder)

Creates a location sort descriptor from a serialized instance.

### Accessing the Location Value

var relativeLocation: CLLocation

The reference location for sorting records.

## Relationships

### Inherits From

- NSSortDescriptor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

## See Also

### Queries

class CKQuery

A query that describes the criteria to apply when searching for records in a database.

class CKQueryOperation

An operation for executing queries in a database.

