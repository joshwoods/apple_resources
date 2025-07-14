

- CKTool JS
-  CKDBRecordChangesResponse 

Structure

# CKDBRecordChangesResponse

An object that represents the results of a record changes lookup operation.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecordChangesResponse {
 CKDBRecordResult[] recordResults;
 boolean moreComing;
 string? changeToken;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecordChangesResponse } from "@apple/cktool.database";
```

## Topics

### Instance Properties

changeToken

A string that identifies a point in the database’s change history.

moreComing

A Boolean value that indicates whether there are more changes to request.

recordResults

An array of record result objects that provide details about the records.

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

CKDBLocation

An object that represents a location field value.

CKDBLookupRecordsRequestBody

An object that represents the request for looking up multiple records by record name.

CKDBLookupRecordsResponse

An object that represents the results of a batch record lookup operation.

CKDBModifyRecordRequestBody

An object that represents the request for updating an existing record.

