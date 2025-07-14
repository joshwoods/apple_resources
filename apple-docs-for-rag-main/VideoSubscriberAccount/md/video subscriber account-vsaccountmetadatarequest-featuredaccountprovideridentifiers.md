

- Video Subscriber Account
- VSAccountMetadataRequest
-  featuredAccountProviderIdentifiers 

Instance Property

# featuredAccountProviderIdentifiers

The providers your app lists prominently during authentication.

iOS 11.0+iPadOS 11.0+macOStvOS 11.0+visionOS 1.0+

``` source
var featuredAccountProviderIdentifiers: [String] { get set }
```

## Discussion

Use this property to specify which providers your app gives prominent placement to when it asks the user to choose an account provider for authentication. By default, no providers are promoted.

## See Also

### Specifying Additional Options

var isInterruptionAllowed: Bool

A Boolean value that indicates whether your app can prompt the user to authenticate to complete the request.

var forceAuthentication: Bool

A Boolean value that indicates whether the app ignores cached credentials.

var localizedVideoTitle: String?

A short, user-presentable name for the video that the user wants to play.

var applicationAccountProviders: [VSAccountApplicationProvider]?

An array of application-specific providers to add to the list of account providers.

