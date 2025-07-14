

- CKTool JS
-  CKDBAssetUploadUrlResponse 

Structure

# CKDBAssetUploadUrlResponse

An object that represents the results of creating an asset upload URL.

CKTool JS 1.2.15+

``` source
dictionary CKDBAssetUploadUrlResponse {
 string url;
};
```

## Overview

You can submit your asset to the URL provided in this response via an HTTP POST request.

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBAssetUploadUrlResponse } from "@apple/cktool.database";
```

## Topics

### Instance Properties

url

The URL for uploading your asset.

## See Also

### Structures

CKDBAsset

An object that represents an asset uploaded to CloudKit.

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

CKDBNullableReference

An object that represents a reference to another record.

