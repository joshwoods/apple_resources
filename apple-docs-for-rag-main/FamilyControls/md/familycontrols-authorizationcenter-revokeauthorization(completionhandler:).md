

- FamilyControls
- AuthorizationCenter
-  revokeAuthorization(completionHandler:) 

Instance Method

# revokeAuthorization(completionHandler:)

Revokes authorization to provide parental controls.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
func revokeAuthorization(completionHandler: @escaping (Result) -> Void)
```

## Parameters 

`completionHandler`  

A closure the system calls after it completes the authorization request. The system passes the following parameters:

`result`  
A value that represents either a success or a failure, including an associated Error object for failures.

## Discussion

If your app’s authentication status is AuthorizationStatus.approved this method revokes authentication.

Note

This method has no effect if your app’s current authentication status is AuthorizationStatus.denied.

The completion handler’s Result parameter indicates whether the request completed successfully. It doesn’t indicate your app’s authorization state.

After you revoke authorization, your app no longer provides parental controls, and the system no longer enforces restrictions, such as preventing the user from deleting your app.

## See Also

### Requesting and Revoking Authorization

func requestAuthorization(for: FamilyControlsMember) async throws

Requests authorization to provide parental controls for a child or individual.

func requestAuthorization(completionHandler: (Result&lt;Void, any Error>) -> Void)

Requests authorization to provide parental controls for a child.

Deprecated

