

- CKTool JS
-  CKDBRecord 

Structure

# CKDBRecord

An object that represents a record in a database.

CKTool JS 1.2.15+

``` source
dictionary CKDBRecord {
 string recordName;
 string recordType;
 string recordChangeTag;
 CKDBChangeMetadata created;
 CKDBChangeMetadata modified;
 dictionary fields;
 dictionary? otherSystemFields;
 CKDBNullableReference? share;
 CKDBNullableReference? parent;
 string? shortGuid;
 CKDBPermissionType? publicPermission;
 CKDBShareParticipant[]? participants;
 CKDBShareParticipant? owner;
 CKDBShareParticipant? currentUserParticipant;
 CKDBStableUrl? stableUrl;
 CKDBZoneId? zone;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBRecord } from "@apple/cktool.database";
```

## Topics

### Instance Properties

created

currentUserParticipant

fields

The dictionary of key-value pairs whose keys are the record field names and values are field-value dictionaries.

modified

otherSystemFields

owner

parent

participants

The array of participants in the shared record.

publicPermission

recordChangeTag

A string that contains the server change token for the record.

recordName

The unique name used to identify the record within a zone.

recordType

The name of the record type.

share

shortGuid

A global unique identifier for this record used for sharing.

stableUrl

zone

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

