

- CKTool JS
-  CKDBStreamingAsset 

Structure

# CKDBStreamingAsset

A streaming asset object that represents a streaming asset in CloudKit.

CKTool JS 1.2.15+

``` source
dictionary CKDBStreamingAsset {
 string? fileSignature;
 string? referenceSignature;
 string? uploadReceipt;
 string? downloadUrl;
 Int64? requestedSize;
 Int64? uploadedSize;
 Int64? reservedSize;
};
```

## Overview

CKDBStreamingAsset is used to start asset upload with minimal data.

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBStreamingAsset } from "@apple/cktool.database";
```

## Topics

### Instance Properties

downloadUrl

The URL for accessing the asset.

fileSignature

The signature of a file returned from the file upload step.

referenceSignature

The signature of a file returned from the asset upload step.

requestedSize

The requested size of streaming asset.

reservedSize

The reserved size of streaming asset.

uploadReceipt

The receipt for uploading the asset.

uploadedSize

The uploaded size of streaming asset.

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

