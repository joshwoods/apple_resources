

- CKTool JS
-  CKDBLocation 

Structure

# CKDBLocation

An object that represents a location field value.

CKTool JS 1.2.15+

``` source
dictionary CKDBLocation {
 Double latitude;
 Double longitude;
 Double? altitude;
 Double? horizontalAccuracy;
 Double? verticalAccuracy;
 Double? course;
 Double? speed;
 date? timestamp;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBLocation } from "@apple/cktool.database";
```

## Topics

### Instance Properties

altitude

The altitude measured in meters.

course

The direction in which the device is traveling.

horizontalAccuracy

The radius of uncertainty for the location measured in meters.

latitude

The latitude of the coordinate point.

longitude

The longitude of the coordinate point.

speed

The instantaneous speed of the device in meters per second.

timestamp

The time at which this location was determined.

verticalAccuracy

The validity of the altitude values and their estimated uncertainty measured in meters.

## See Also

### Structures

CKDBAsset

An object that represents an asset uploaded to CloudKit.

CKDBAssetUploadUrlResponse

An object that represents the results of creating an asset upload URL.

CKDBChangeMetadata

An object that represents metadata about a record change via creation or modification.

CKDBCreateAssetUploadUrlRequestBody

An object that represents the request for creating an asset upload URL.

CKDBCreateRecordRequestBody

An object that represents the request to create a new record.

CKDBCreateZoneRequestBody

An object that represents the request to create a new zone.

CKDBDeleteRecordsByQueryRequestBody

An object that represents the request to delete multiple records that match a query.

CKDBDeletedRecordResult

An object that represents a deleted record result.

CKDBErrorRecordResult

An object that represents a record lookup failure.

CKDBExistingRecordResult

An object that represents a successful record result.

CKDBForRecord

An object that represents a record that is being shared.

CKDBLookupRecordsRequestBody

An object that represents the request for looking up multiple records by record name.

CKDBLookupRecordsResponse

An object that represents the results of a batch record lookup operation.

CKDBModifyRecordRequestBody

An object that represents the request for updating an existing record.

CKDBNullableReference

An object that represents a reference to another record.

