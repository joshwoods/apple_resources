

- CKTool JS
-  CKDBChangeMetadata 

Structure

# CKDBChangeMetadata

An object that represents metadata about a record change via creation or modification.

CKTool JS 1.2.15+

``` source
dictionary CKDBChangeMetadata {
 string? deviceId;
 date timestamp;
 string userRecordName;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBChangeMetadata } from "@apple/cktool.database";
```

## Topics

### Instance Properties

deviceId

The device where the change occurred.

timestamp

The time of the change.

userRecordName

The record name that represents the user who made the change.

## See Also

### Structures

CKDBAsset

An object that represents an asset uploaded to CloudKit.

CKDBAssetUploadUrlResponse

An object that represents the results of creating an asset upload URL.

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

CKDBLocation

An object that represents a location field value.

CKDBLookupRecordsRequestBody

An object that represents the request for looking up multiple records by record name.

CKDBLookupRecordsResponse

An object that represents the results of a batch record lookup operation.

CKDBModifyRecordRequestBody

An object that represents the request for updating an existing record.

CKDBNullableReference

An object that represents a reference to another record.

