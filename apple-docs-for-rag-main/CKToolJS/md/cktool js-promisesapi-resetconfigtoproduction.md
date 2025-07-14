

- CKTool JS
- PromisesApi
-  resetConfigToProduction 

Instance Method

# resetConfigToProduction

Resets the container configuration to production.

CKTool JS 1.2.15+

``` source
CancellablePromise resetConfigToProduction(
 ResetConfigToProductionParams params
);
```

## Parameters 

`params`  

A dictionary as described in the Discussion section.

## Return Value

A `CancellablePromise` with the following resolutions.

## Discussion

If the promise is successful, it will resolve with one of the following dictionaries:

- `{ statusCode: 202 }`

The promise may reject and throw the following:

- `DocumentedResponseError`, if the HTTP status code is 421. The result member will be a dictionary conforming to AuthenticationRequiredError.

- `DocumentedResponseError`, if the HTTP status code is none of the above and in the range 400 to 599. The result member will be a dictionary conforming to RequestError.

- `ValidationError`, if the parameters to the method are incorrect.

- A `FetchError` descendant, if there is a problem with the network request. A reference to the request object can be used to examine the underlying cause.

## Discussion

The `params` dictionary has the following properties:

```
dictionary ResetConfigToProductionParams {
  string teamId;
  string containerId;
}
```

- `teamId`: The team identifier. You can find your team identifier in the Membership tab of the Apple Developer portal at `https://developer.apple.com`.

- `containerId`: The container identifier. See `Container`.

## See Also

### Database Management

exportSchema

Downloads the container’s schema.

getContainers

Fetches containers for a team.

importSchema

Uploads a file that defines the new schema for the container.

resetToProduction

Resets the schema of the environment to production.

validateSchema

Validates the uploaded schema file for the container.

