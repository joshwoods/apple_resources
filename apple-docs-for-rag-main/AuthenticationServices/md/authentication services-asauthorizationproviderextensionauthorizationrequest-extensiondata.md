

- Authentication Services
- ASAuthorizationProviderExtensionAuthorizationRequest
-  extensionData 

Instance Property

# extensionData

Extension data from the Mobile Device Management (MDM) configuration.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS 1.0+

``` source
var extensionData: [AnyHashable : Any] { get }
```

## See Also

### Getting Context

var callerBundleIdentifier: String

The bundle ID of the app making the request.

var callerTeamIdentifier: String

The team identifier of the app making the request.

var localizedCallerDisplayName: String

The localized display name of the app making the request.

var isCallerManaged: Bool

A Boolean value that indicates whether the app making the request is managed.

