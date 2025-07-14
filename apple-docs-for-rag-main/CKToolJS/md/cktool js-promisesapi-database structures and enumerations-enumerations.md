

- CKTool JS
- PromisesApi
-  Database Structures and Enumerations 

API Collection

# Database Structures and Enumerations

## Topics

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

CKDBNullableReference

An object that represents a reference to another record.

CKDBPagedBatchDeleteResponse

An object that represents the results of a paginated batch delete operation.

CKDBQuery

An object that represents a query for searching records.

CKDBQueryFilter

An object that represents the logical conditions for determining whether a record matches the query.

CKDBQueryRecordsRequestBody

An object that represents the request for fetching multiple records that match a query.

CKDBQuerySort

An object that represents a sort descriptor that specifies how to order fetched records.

CKDBRecord

An object that represents a record in a database.

CKDBRecordChangesRequestBody

An object that represents the request for fetching changes since a specified zone change token.

CKDBRecordChangesResponse

An object that represents the results of a record changes lookup operation.

CKDBRecordReference

An object that represents a reference to a CloudKit database record.

CKDBRecordResponse

An object that represents the results of a record lookup operation.

CKDBRecordResult

An object that represents a record when the lookup operation can potentially return deleted records or fail partially when looking up some of the record.

CKDBRecordsResponse

An object that represents the results of a batch record lookup operation.

CKDBResolveRecordRequestBody

An object that represents a request for fetching a record given its `shortGuid`.

CKDBResolveRecordResponse

An object that represents the results of looking up a record by its `shortGuid`.

CKDBResolvedRecord

An object that represents a shared record fetched using its `shortGuid`.

CKDBSchemaImportRequestBody

An object that contains a schema file to be applied to a container environment.

CKDBSessionUser

An object that represents the current user.

CKDBSessionUserResponse

An object that contains the result of looking up the current user.

CKDBShareParticipant

An object that represents a share participant.

CKDBSharePotentialParticipant

An object that represents a potential participant for a share.

CKDBStableUrl

Internal use only.

CKDBStreamingAsset

A streaming asset object that represents a streaming asset in CloudKit.

CKDBUserIdentity

An object that identifies a user participating in a share.

CKDBUserIdentityLookupInfo

An object that represents lookup information for a user.

CKDBUserNameComponents

An object that represents the user’s name.

CKDBValidateSchemaResponse

The response object after validating the uploaded schema string.

CKDBZone

An object that represents a CloudKit database zone.

CKDBZoneId

An object that represents a CloudKit database zone identifier.

CKDBZoneResponse

An object that represents results of fetching a zone.

CKDBZonesResponse

An object that represents results of fetching multiple zones.

### Enumerations

CKDBPermissionType

The participant’s read and write permissions.

CKDBQueryFilterType

An object that represents the type of a filter that indicates the comparison operator when applying the filter.

CKDBQuerySortOrder

An enumeration that represents the order to use when sorting records.

CKDBRecordReferenceAction

An object that represents the action to be performed for the referenced record.

CKDBShareAcceptanceStatus

An enumeration that indicates the status of accepting the shared record.

CKDBShareParticipantType

An enumeration that represents the type of a share participant.

## See Also

### Database Field Values, Structures and Enumerations

Field Values

