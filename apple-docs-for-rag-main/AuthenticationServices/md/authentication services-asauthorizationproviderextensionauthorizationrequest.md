

- Authentication Services
-  ASAuthorizationProviderExtensionAuthorizationRequest 

Class

# ASAuthorizationProviderExtensionAuthorizationRequest

An authorization request that your provider extension handles.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
class ASAuthorizationProviderExtensionAuthorizationRequest
```

## Topics

### Parsing the Request

var url: URL

The complete URL of the request, including all components.

var httpHeaders: [String : String]

The HTTP headers of the request.

var httpBody: Data

The HTTP body of the request.

var realm: String

The realm to which the request applies.

var requestedOperation: ASAuthorizationProviderAuthorizationOperation

The operation for the extension to execute.

struct ASAuthorizationProviderAuthorizationOperation

A type that represents an authorization operation.

var authorizationOptions: [AnyHashable : Any]

A collection of options associated with the request.

### Getting Context

var callerBundleIdentifier: String

The bundle ID of the app making the request.

var callerTeamIdentifier: String

The team identifier of the app making the request.

var localizedCallerDisplayName: String

The localized display name of the app making the request.

var isCallerManaged: Bool

A Boolean value that indicates whether the app making the request is managed.

var extensionData: [AnyHashable : Any]

Extension data from the Mobile Device Management (MDM) configuration.

### Interacting with the User

func presentAuthorizationViewController(completion: (Bool, (any Error)?) -> Void)

Asks the authorization service to show the extension’s view controller to the user.

var isUserInterfaceEnabled: Bool

Determines if user interface is available for the current request.

### Completing a Request

func complete(authorizationResult: ASAuthorizationProviderExtensionAuthorizationResult)

func complete()

Indicates the requested authorization completed with no output.

func complete(httpAuthorizationHeaders: [String : String])

Indicates the requested authorization succeeded with tokens in the HTTP headers.

func complete(httpResponse: HTTPURLResponse, httpBody: Data?)

Indicates the requested authorization succeeded with an HTTP response.

func complete(error: any Error)

Indicates the requested authorization failed.

### Canceling a Request

func doNotHandle()

Indicates the request wasn’t handled.

func cancel()

Cancels the request, for example, because the user taps a cancel button.

### Supporting Platform Single Sign-On

var loginManager: ASAuthorizationProviderExtensionLoginManager?

The manager that interacts with Platform SSO.

### Instance Properties

var callerAuditToken: Data

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Starting or Canceling a Request

func beginAuthorization(with: ASAuthorizationProviderExtensionAuthorizationRequest)

Tells your request handler to authorize the given request.

**Required**

func cancelAuthorization(with: ASAuthorizationProviderExtensionAuthorizationRequest)

Tells your request handler to cancel the authorization of the given request.

