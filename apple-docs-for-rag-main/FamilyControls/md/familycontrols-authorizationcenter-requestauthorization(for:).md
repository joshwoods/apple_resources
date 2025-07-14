

- FamilyControls
- AuthorizationCenter
-  requestAuthorization(for:) 

Instance Method

# requestAuthorization(for:)

Requests authorization to provide parental controls for a child or individual.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
func requestAuthorization(for member: FamilyControlsMember) async throws
```

## Parameters 

`member`  

The FamilyControlsMember that requests authorization

## Discussion

With this function you can authorize parental controls for a FamilyControlsMember.child that’s signed into the iCloud account on the device or a FamilyControlsMember.individual. A parent or guardian must authenticate a child’s account, while individuals can authenticate their own account. For more information, see FamilyControlsMember.

Call this method when your app first launches.

If the FamilyControlsMember.individual hasn’t authorized your app previously, the device tries to authorize that individual using Face ID or Touch ID. After the user approves or cancels the request, the system either sets the authorization status or throws an error.

After a FamilyControlsMember.individual authorizes your app, additional calls to `requestAuthorization(for:)` no longer ask to authorize that `individual` using Face ID or Touch ID. Additionally, the system removes any restrictions that prevent the user from bypassing parental controls so the user can delete an authorized app or sign out of iCloud as needed.

You can revoke authorization by calling revokeAuthorization(completionHandler:).

## See Also

### Requesting and Revoking Authorization

func revokeAuthorization(completionHandler: (Result&lt;Void, any Error>) -> Void)

Revokes authorization to provide parental controls.

func requestAuthorization(completionHandler: (Result&lt;Void, any Error>) -> Void)

Requests authorization to provide parental controls for a child.

Deprecated

