

- CKTool JS
- PromisesApi
-  resolveRecord 

Instance Method

# resolveRecord

Fetches information about records given their shortGuid properties.

CKTool JS 1.2.15+

``` source
CancellablePromise resolveRecord(
 ResolveRecordParams params
);
```

## Parameters 

`params`  

A dictionary as described in the Discussion section.

## Return Value

A `CancellablePromise` with the following resolutions.

## Discussion

If the promise is successful, it will resolve with one of the following dictionaries:

- `{ statusCode: 200; result: CKDBResolveRecordResponse }`

The promise may reject and throw the following:

- `DocumentedResponseError`, if the HTTP status code is 421. The result member will be a dictionary conforming to AuthenticationRequiredError.

- `DocumentedResponseError`, if the HTTP status code is none of the above and in the range 400 to 599. The result member will be a dictionary conforming to RequestError.

- `ValidationError`, if the parameters to the method are incorrect.

- A `FetchError` descendant, if there is a problem with the network request. A reference to the request object can be used to examine the underlying cause.

## Discussion

The `params` dictionary has the following properties:

```
dictionary ResolveRecordParams {
  string containerId;
  CKEnvironment environment;
  string shortGuid;
  CKDBResolveRecordRequestBody? body;
}
```

- `containerId`: The container identifier. See `Container`.

- `environment`: The container environment. For valid values, see `CKEnvironment`.

- `shortGuid`: A global unique identifier for this record used for sharing. See `createRecord` for information on retrieving this identifier.

- `body`: Configuration options for how the resolved record is returned.

If successful, the response contains a `CKDBResolveRecordResponse` object with the resolved record.

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

getRecord

Returns a record’s details.

lookupRecords

Fetches multiple records by record name.

queryRecordChanges

Returns records that changed since a specified sync token or since a zone was created.

queryRecords

Returns a collection of records matching the provided query.

updateRecord

Updates an existing record.

