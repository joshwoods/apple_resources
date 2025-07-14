

- FamilyControls
- AuthorizationCenter
-  requestAuthorization(completionHandler:) Deprecated

Instance Method

# requestAuthorization(completionHandler:)

Requests authorization to provide parental controls for a child.

iOS 15.0–16.0DeprecatediPadOS 15.0–16.0DeprecatedMac Catalyst 15.0–16.0Deprecated

``` source
func requestAuthorization(completionHandler: @escaping (Result) -> Void)
```

Deprecated

Use requestAuthorization(for:) instead.

## Parameters 

`completionHandler`  

A closure the system calls after it completes the authorization request.

## See Also

### Requesting and Revoking Authorization

func requestAuthorization(for: FamilyControlsMember) async throws

Requests authorization to provide parental controls for a child or individual.

func revokeAuthorization(completionHandler: (Result&lt;Void, any Error>) -> Void)

Revokes authorization to provide parental controls.

