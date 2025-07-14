

- CKTool JS
- PromisesApi
-  deleteRecordsByQuery 

Instance Method

# deleteRecordsByQuery

Deletes records matching the provided query.

CKTool JS 1.2.15+

``` source
CancellablePromise deleteRecordsByQuery(
 DeleteRecordsByQueryParams params
);
```

## Parameters 

`params`  

A dictionary as described in the Discussion section.

## Return Value

A `CancellablePromise` with the following resolutions.

## Discussion

If the promise is successful, it will resolve with one of the following dictionaries:

- `{ statusCode: 200; result: CKDBPagedBatchDeleteResponse }`

The promise may reject and throw the following:

- `DocumentedResponseError`, if the HTTP status code is 421. The result member will be a dictionary conforming to AuthenticationRequiredError.

- `DocumentedResponseError`, if the HTTP status code is none of the above and in the range 400 to 599. The result member will be a dictionary conforming to RequestError.

- `ValidationError`, if the parameters to the method are incorrect.

- A `FetchError` descendant, if there is a problem with the network request. A reference to the request object can be used to examine the underlying cause.

## Discussion

The `params` dictionary has the following properties:

```
dictionary DeleteRecordsByQueryParams {
  CKDBDeleteRecordsByQueryRequestBody body;
  string containerId;
  CKEnvironment environment;
  string databaseType;
  string zoneName;
}
```

- `body`: Query and other options for the delete records operation.

- `containerId`: The container identifier. See `Container`.

- `environment`: The container environment. For valid values, see `CKEnvironment`.

- `databaseType`: The database type. For valid values, see `CKDatabaseType`.

- `zoneName`: The zone name. See `CKDBZone`.

This operation allows you to delete multiple records of a record type that match specific filters. If the operation completes, the response contains a `CKDBPagedBatchDeleteResponse` object that details the result of the batch delete operation. You can delete up to 200 records in a single operation. If more records match your filters, the response also contains a continuation token that you can use to delete the next set of matching records.

## See Also

### Record Management

acceptRecord

Accepts a share on behalf of the current user.

createRecord

Creates a new record.

deleteRecord

Deletes a single record.

getRecord

Returns a record’s details.

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

