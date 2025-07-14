

- FamilyControls
-  AuthorizationCenter 

Class

# AuthorizationCenter

The center for requesting authorization to provide parental controls.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
class AuthorizationCenter
```

## Overview

To authorize your app so that it can provide parental controls, access the shared `AuthorizationCenter` instance.

```
let center = AuthorizationCenter.shared
```

Important

You must add the Family Controls capability to your app before you call the requestAuthorization(for:) or revokeAuthorization(completionHandler:) methods. This capability adds the Family Controls entitlement to your app. In a compatible iPad or iPhone app running in visionOS, authorization attempts always fail. For more information, see Adding capabilities to your app.

Next, to request authorization to provide parental controls, call requestAuthorization(completionHandler:)

```
center.requestAuthorization { result in
    switch result {
    case .success():
        // The request succeeded.
    case .failure(let error):
        // Handle the error here.
    }
}
```

or requestAuthorization(for:).

```
do {
    try await center.requestAuthorization(for: FamilyControlsMember.individual)
} catch {
    // Handle the error here.
}
```

Always request authorization when your app first launches. If the user’s parent or guardian hasn’t previously authorized your app, the system displays an alert. If the parent or guardian chooses to continue, it displays an authentication sheet. When a parent or guardian either approves or cancels the request, the system sends the result back to the `requestAuthorization(completionHandler:)` method’s completion handler.

If you’re authenticating an `individual` who hasn’t previously authorized your app, the system displays an alert. If the `individual` chooses to continue, the device asks to authorize that `individual` using Face ID or Touch ID.

After your app has been authorized, additional calls to `requestAuthorization(for:)` don’t display the authentication sheet or ask to authorize that individual using Face ID or Touch ID. Instead, the system sets the authorization status.

To observe changes to the authorization status, use the authorizationStatus property.

The status may change due to external events, such as a child graduating to an adult account, or a parent or guardian changing the status in Settings. You can also revoke authorization by calling revokeAuthorization(completionHandler:)

## Topics

### Accessing the Shared Center

static let shared: AuthorizationCenter

The shared center for requesting and revoking authorization.

### Requesting and Revoking Authorization

func requestAuthorization(for: FamilyControlsMember) async throws

Requests authorization to provide parental controls for a child or individual.

func revokeAuthorization(completionHandler: (Result&lt;Void, any Error>) -> Void)

Revokes authorization to provide parental controls.

func requestAuthorization(completionHandler: (Result&lt;Void, any Error>) -> Void)

Requests authorization to provide parental controls for a child.

Deprecated

### Tracking Authorization Changes

var authorizationStatus: AuthorizationStatus

The status of your app’s authorization to provide parental controls.

var $authorizationStatus: Published&lt;AuthorizationStatus>.Publisher

A publisher for the authorization status property.

var objectWillChange: ObservableObjectPublisher

typealias ObjectWillChangePublisher

The type of publisher that emits before the object has changed.

### Default Implementations

ObservableObject Implementations

## Relationships

### Conforms To

- ObservableObject

## See Also

### Authorizations

enum AuthorizationStatus

The status of your app’s authorization to provide parental controls.

Family Controls

A Boolean value that indicates whether the app can request or revoke authorization to provide parental controls.

