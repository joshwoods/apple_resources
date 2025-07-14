

- CKTool JS
-  CKDBUserNameComponents 

Structure

# CKDBUserNameComponents

An object that represents the user’s name.

CKTool JS 1.2.15+

``` source
dictionary CKDBUserNameComponents {
 string? givenName;
 string? middleName;
 string? familyName;
 string? namePrefix;
 string? nameSuffix;
 string? nickname;
 string? phoneticRepresentation;
};
```

## Overview

In JavaScript, this is a plain object with properties as described.

In TypeScript, this type is imported in the following way:

```
import type { CKDBUserNameComponents } from "@apple/cktool.database";
```

## Topics

### Instance Properties

familyName

The user’s last name.

givenName

The user’s first name.

middleName

The user’s middle name.

namePrefix

The user’s prefix.

nameSuffix

The user’s suffix.

nickname

The user’s nickname.

phoneticRepresentation

A phonetic representation of the user’s name.

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

