

- CKTool JS
-  CKDBResolvedRecord 

Structure

# CKDBResolvedRecord

An object that represents a shared record fetched using its `shortGuid`.

CKTool JS 1.2.15+

``` source
dictionary CKDBResolvedRecord {
 string shortGuid;
 string? containerId;
 CKEnvironment? environment;
 string? databaseType;
 CKDBZoneId? zone;
 string? rootRecordName;
 CKDBRecord? share;
 CKDBRecord? rootRecord;
 CKDBRecord? resolvedRecord;
 CKDBRecord[]? ancestorRecords;
 CKDBShareParticipantType? participantType;
 CKDBShareAcceptanceStatus? participantStatus;
 CKDBPermissionType? participantPermission;
 CKDBUserIdentity? userIdentity;
 CKDBSharePotentialParticipant[]? potentialMatches;
 string? webpageUrl;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBResolvedRecord } from "@apple/cktool.database";
```

## Topics

### Instance Properties

ancestorRecords

The array of record objects that represent the ancestor records.

containerId

The container identifier.

databaseType

The database type.

environment

participantPermission

participantStatus

participantType

potentialMatches

An array of potential participants that the user can choose from.

resolvedRecord

rootRecord

rootRecordName

The name of the root record that was shared.

share

shortGuid

A global unique identifier for a shared record.

userIdentity

webpageUrl

The fallback URL that you can redirect users to if the operation fails.

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

