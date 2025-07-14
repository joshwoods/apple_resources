

- CKTool JS
- PromisesApi
-  getRecord 

Instance Method

# getRecord

Returns a record’s details.

CKTool JS 1.2.15+

``` source
CancellablePromise getRecord(
 GetRecordParams params
);
```

## Parameters 

`params`  

A dictionary as described in the Discussion section.

## Return Value

A `CancellablePromise` with the following resolutions.

## Discussion

If the promise is successful, it will resolve with one of the following dictionaries:

- `{ statusCode: 200; result: CKDBRecordResponse }`

The promise may reject and throw the following:

- `DocumentedResponseError`, if the HTTP status code is 421. The result member will be a dictionary conforming to AuthenticationRequiredError.

- `DocumentedResponseError`, if the HTTP status code is none of the above and in the range 400 to 599. The result member will be a dictionary conforming to RequestError.

- `ValidationError`, if the parameters to the method are incorrect.

- A `FetchError` descendant, if there is a problem with the network request. A reference to the request object can be used to examine the underlying cause.

## Discussion

The `params` dictionary has the following properties:

```
dictionary GetRecordParams {
  string containerId;
  CKEnvironment environment;
  string databaseType;
  string zoneName;
  string recordName;
  string[]? requestedFields;
}
```

- `containerId`: The container identifier. See `Container`.

- `environment`: The container environment. For valid values, see `CKEnvironment`.

- `databaseType`: The database type. For valid values, see `CKDatabaseType`.

- `zoneName`: The zone name. See `CKDBZone`.

- `recordName`: The record name. See `CKDBRecord`.

- `requestedFields`: The array of record field names that limits the amount of data returned in this operation. The server only returns fields specified in the array.

If successful, the result contains a `CKDBRecordResponse` object with the requested record. If you provide `requestedFields`, the server only returns fields specified in that array. If it’s set to an empty array, the server returns record metadata without the field values. If you omit `requestedFields`, the server returns all record fields.

## See Also

### Record Management

acceptRecord

Accepts a share on behalf of the current user.

createRecord

Creates a new record.

deleteRecord

Deletes a single record.

deleteRecordsByQuery

Deletes records matching the provided query.

lookupRecords

Fetches multiple records by record name.

queryRecordChanges

Returns records that changed since a specified sync token or since a zone was created.

queryRecords

Returns a collection of records matching the provided query.

resolveRecord

Fetches information about records given their shortGuid properties.

updateRecord

Updates an existing record.

