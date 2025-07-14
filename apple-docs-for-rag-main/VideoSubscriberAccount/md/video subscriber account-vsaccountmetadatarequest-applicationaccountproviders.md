

- Video Subscriber Account
- VSAccountMetadataRequest
-  applicationAccountProviders 

Instance Property

# applicationAccountProviders

An array of application-specific providers to add to the list of account providers.

iOS 14.2+iPadOS 14.2+macOStvOS 14.2+visionOS 1.0+

``` source
var applicationAccountProviders: [VSAccountApplicationProvider]? { get set }
```

## See Also

### Specifying Additional Options

var isInterruptionAllowed: Bool

A Boolean value that indicates whether your app can prompt the user to authenticate to complete the request.

var featuredAccountProviderIdentifiers: [String]

The providers your app lists prominently during authentication.

var forceAuthentication: Bool

A Boolean value that indicates whether the app ignores cached credentials.

var localizedVideoTitle: String?

A short, user-presentable name for the video that the user wants to play.

