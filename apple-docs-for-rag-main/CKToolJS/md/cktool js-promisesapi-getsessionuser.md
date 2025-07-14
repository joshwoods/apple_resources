

- CKTool JS
- PromisesApi
-  getSessionUser 

Instance Method

# getSessionUser

Returns details for the user in current session.

CKTool JS 1.2.15+

``` source
CancellablePromise getSessionUser(
 GetSessionUserParams params
);
```

## Parameters 

`params`  

A dictionary as described in the Discussion section.

## Return Value

A `CancellablePromise` with the following resolutions.

## Discussion

If the promise is successful, it will resolve with one of the following dictionaries:

- `{ statusCode: 200; result: CKDBSessionUserResponse }`

The promise may reject and throw the following:

- `DocumentedResponseError`, if the HTTP status code is 421. The result member will be a dictionary conforming to AuthenticationRequiredError.

- `DocumentedResponseError`, if the HTTP status code is none of the above and in the range 400 to 599. The result member will be a dictionary conforming to RequestError.

- `ValidationError`, if the parameters to the method are incorrect.

- A `FetchError` descendant, if there is a problem with the network request. A reference to the request object can be used to examine the underlying cause.

## Discussion

The `params` dictionary has the following properties:

```
dictionary GetSessionUserParams {
  string containerId;
  CKEnvironment environment;
}
```

- `containerId`: The container identifier. See `Container`.

- `environment`: The container environment. For valid values, see `CKEnvironment`.

If successful, the returned response contains a `CKDBSessionUserResponse` object with the current user information. If the user hasn’t authenticated yet or if their authentication has expired, the server returns an `AuthenticationRequiredError` error with a `redirectUrl` that your app can use to re-authenticate the user.

## See Also

### User and Team

getTeams

Fetches a list of teams the current user is in.

Team

Details of a developer team.

TeamsResponse

Response object for a list of teams.

