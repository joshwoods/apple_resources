

- CKTool JS
-  CKDBZone 

Structure

# CKDBZone

An object that represents a CloudKit database zone.

CKTool JS 1.2.15+

``` source
dictionary CKDBZone {
 string zoneName;
 string canonicalName;
 string zoneType;
 boolean isDefaultZone;
 boolean? isSharable;
 boolean? isEligibleForZoneShare;
 boolean? isEligibleForHierarchicalShare;
 string? ownerRecordName;
 string? changeToken;
 boolean atomic;
};
```

## Overview

A zone is a logical separation of records within a single database. Features are often associated with an entire zone. For example, a zone may be optionally shared from one user to another.

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBZone } from "@apple/cktool.database";
```

## Topics

### Instance Properties

atomic

A Boolean value that indicates whether a zone allows atomic changes of multiple records.

canonicalName

The unique identifier for a zone within a database.

changeToken

The client change token for the zone.

isDefaultZone

A Boolean value that indicates whether the zone is a default zone.

isEligibleForHierarchicalShare

A Boolean value that indicates whether zone is eligible for Hierarchical Share.

isEligibleForZoneShare

A Boolean value that indicates whether zone is eligible for Zone Share.

isSharable

A Boolean value that indicates whether records in this zone can be shared.

ownerRecordName

The owner of the zone.

zoneName

The name that identifies the record zone.

zoneType

The type for the zone.

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

