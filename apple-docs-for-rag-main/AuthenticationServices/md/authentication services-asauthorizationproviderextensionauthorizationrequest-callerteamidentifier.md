

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  callerTeamIdentifier 

Instance Property

# callerTeamIdentifier

The team identifier of the app making the request.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var callerTeamIdentifier: String { get }
```

## See Also

### Getting Context

var callerBundleIdentifier: String

The bundle ID of the app making the request.

var localizedCallerDisplayName: String

The localized display name of the app making the request.

var isCallerManaged: Bool

A Boolean value that indicates whether the app making the request is managed.

var extensionData: [AnyHashable : Any]

Extension data from the Mobile Device Management (MDM) configuration.

