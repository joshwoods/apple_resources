

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  isCallerManaged 

Instance Property

# isCallerManaged

A Boolean value that indicates whether the app making the request is managed.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var isCallerManaged: Bool { get }
```

## See Also

### Getting Context

var callerBundleIdentifier: String

The bundle ID of the app making the request.

var callerTeamIdentifier: String

The team identifier of the app making the request.

var localizedCallerDisplayName: String

The localized display name of the app making the request.

var extensionData: [AnyHashable : Any]

Extension data from the Mobile Device Management (MDM) configuration.

