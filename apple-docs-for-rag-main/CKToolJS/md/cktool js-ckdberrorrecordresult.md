

- CKTool JS
-  CKDBErrorRecordResult 

Structure

# CKDBErrorRecordResult

An object that represents a record lookup failure.

CKTool JS 1.2.15+

``` source
dictionary CKDBErrorRecordResult {
 string type;
 string? recordName;
 string errorCode;
 string message;
};
```

## Overview

The server returns a CKDBErrorRecordResult object when looking up a record fails as part of a batch record lookup operation.

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBErrorRecordResult } from "@apple/cktool.database";
```

## Topics

### Instance Properties

errorCode

A string containing the code for the error that occurred.

message

A string that indicates the reason for the error.

recordName

The name of the record.

type

The type of the record result.

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

