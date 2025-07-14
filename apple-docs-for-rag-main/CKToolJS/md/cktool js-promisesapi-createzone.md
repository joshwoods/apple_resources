

- CKTool JS
- PromisesApi
-  createZone 

Instance Method

# createZone

Creates a new zone.

CKTool JS 1.2.15+

``` source
CancellablePromise createZone(
 CreateZoneParams params
);
```

## Parameters 

`params`  

A dictionary as described in the Discussion section.

## Return Value

A `CancellablePromise` with the following resolutions.

## Discussion

If the promise is successful, it will resolve with one of the following dictionaries:

- `{ statusCode: 201; result: CKDBZoneResponse }`

The promise may reject and throw the following:

- `DocumentedResponseError`, if the HTTP status code is 421. The result member will be a dictionary conforming to AuthenticationRequiredError.

- `DocumentedResponseError`, if the HTTP status code is none of the above and in the range 400 to 599. The result member will be a dictionary conforming to RequestError.

- `ValidationError`, if the parameters to the method are incorrect.

- A `FetchError` descendant, if there is a problem with the network request. A reference to the request object can be used to examine the underlying cause.

## Discussion

The `params` dictionary has the following properties:

```
dictionary CreateZoneParams {
  CKDBCreateZoneRequestBody body;
  string containerId;
  CKEnvironment environment;
  string databaseType;
}
```

- `body`: New zone details.

- `containerId`: The container identifier. See `Container`.

- `environment`: The container environment. For valid values, see `CKEnvironment`.

- `databaseType`: The database type. For valid values, see `CKDatabaseType`.

If successful, the result contains a `CKDBZoneResponse` object with the created zone.

## See Also

### Zone Management

deleteZone

Deletes a zone.

getZone

Returns details for a zone.

getZones

Returns a collection of zones.

