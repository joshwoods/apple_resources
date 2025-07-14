

- CKTool JS
-  CKDBDeleteRecordsByQueryRequestBody 

Structure

# CKDBDeleteRecordsByQueryRequestBody

An object that represents the request to delete multiple records that match a query.

CKTool JS 1.2.15+

``` source
dictionary CKDBDeleteRecordsByQueryRequestBody {
 boolean? dryRun;
 string recordType;
 CKDBQueryFilter[]? filters;
 Int32? resultsLimit;
 string? continuationToken;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBDeleteRecordsByQueryRequestBody } from "@apple/cktool.database";
```

## Topics

### Instance Properties

continuationToken

The location of the last batch of results.

dryRun

A Boolean value that indicates whether to delete matching records.

filters

The array of filters to apply when querying records for deletion.

recordType

The record type to use when performing the query.

resultsLimit

The maximum number of records to delete.

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

