

- CKTool JS
-  CKDBModifyRecordRequestBody 

Structure

# CKDBModifyRecordRequestBody

An object that represents the request for updating an existing record.

CKTool JS 1.2.15+

``` source
dictionary CKDBModifyRecordRequestBody {
 string recordType;
 string? recordChangeTag;
 dictionary fields;
 boolean? createShortGuid;
 CKDBNullableReference? share;
 CKDBNullableReference? parent;
 CKDBForRecord? forRecord;
 CKDBPermissionType? publicPermission;
 CKDBShareParticipant[]? participants;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBModifyRecordRequestBody } from "@apple/cktool.database";
```

## Topics

### Instance Properties

createShortGuid

A Boolean value that indicates whether to create a short GUID for sharing this record.

fields

The dictionary of key-value pairs whose keys are the record field names and values are field-value dictionaries.

forRecord

parent

participants

The array of participants in the shared record.

publicPermission

recordChangeTag

A string containing the server change token for the record.

recordType

The name of the record type.

share

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

CKDBNullableReference

An object that represents a reference to another record.

